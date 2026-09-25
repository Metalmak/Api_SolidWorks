<!-- source: sldworksapi/Create_Advanced_Hole_Example_VB.htm -->

# SOLIDWORKS API Help

# Create Advanced Hole Feature Example (VBA)

This example shows how to create an Advanced Hole feature.

'----------------------------------------------------------------------------

' Preconditions:
' 1. Verify that the specified part document exists.
' 2. Open the Immediate window.
'
' Postconditions:
' 1. Selects near and far side faces of the Advanced Hole.
' 2. Defines an Advanced Hole at a sketch point on the edge of the block
'    with the following:
'    \* Countersink near side element
'    \* Straight tap near side element
'    \* Counterbore far side element
'    \* Straight hole far side element
' 3. Gets some near and far side element data for the Advanced Hole.
' 4. Modifies the near side element array to contain a tapered tap element.
' 5. Deletes the Advanced Hole's defining sketch point on the edge of the block.
' 6. Adds two sketch points and creates two Advanced Holes at those locations
'    using the previously defined Advanced Hole.
' 7. Inspect the Immediate window and graphics area.
'
' NOTE: Because the model is used elsewhere, do not save changes.
'----------------------------------------------------------------------------

Option Explicit

Dim swApp As SldWorks.SldWorks
Dim swModel As SldWorks.ModelDoc2
Dim feat As Feature
Dim boolstatus As Boolean
Dim swAdvHole\_Near\_1 As AdvancedHoleElementData
Dim swAdvHole\_Near\_2 As AdvancedHoleElementData
Dim swAdvHole\_Near\_3 As AdvancedHoleElementData
Dim swAdvHole\_Far\_1 As AdvancedHoleElementData
Dim swAdvHole\_Far\_2 As AdvancedHoleElementData
Dim swCounterSinkNear As CountersinkElementData
Dim swCounterBoreFar As CounterboreElementData
Dim swStraightHoleFar As StraightElementData
Dim swStraightTapNear As StraightTapElementData
Dim swTaperedTapNear As TaperedTapElementData
Dim swFeatureMgr As FeatureManager
Dim ConvFactorAngle, ConvFactorLength As Double
Dim advHoleNearArr(1) As AdvancedHoleElementData
Dim advHoleFarArr(1) As AdvancedHoleElementData
Dim featdata As AdvancedHoleFeatureData
Dim newNearArr(1) As AdvancedHoleElementData
Dim newFarArr(1) As AdvancedHoleElementData
Dim swSketchFeature As Feature
Dim swSelectionManager As SelectionMgr
Dim swSketch As Sketch
Dim swSketchPointArray As Variant
Dim swMaxPointNumber As Long
Dim skPoint As Object
Dim swSketchPoint As Object
Dim swCurrentPointNumber As Long
Dim errors As Long, warnings As Long
Dim jtr As Long
Dim ResultArray As Variant
Dim CalloutString As String
Dim StrDiam As String
Dim strDepth As String
Dim retVal as Boolean

Sub main()

    Set swApp = Application.SldWorks
    Set swModel = swApp.**OpenDoc6**("C:\Users\Public\Documents\SOLIDWORKS\SOLIDWORKS
2018\samples\tutorial\api\block20.sldprt", swDocPART, swOpenDocOptions\_Silent, "",
errors, warnings)
    Set swFeatureMgr = swModel.**FeatureManager**
    ConvFactorLength = 25.4 / 1000 'inches to meters
    ConvFactorAngle = (22 / 7) / 180 'degrees to radians

    'Select the near and far side faces
    boolstatus = swModel.**Extension**.**SelectByRay**(-5.89202612791269E-02,
2.60626824463657E-02, 5.60000000000969E-02, -0.400036026779312,
-0.515038074910024, -0.758094294050284, 7.22831189342222E-04, 2, False, 256, 0)
'Near side
    boolstatus = swModel.**Extension**.**SelectByRay**(-1.10716643645077E-02,
2.11784489308116E-02, -6.39370439421896E-02, 0.18261953966356,
-0.612697461661826, 0.76892907618728, 9.36301020408163E-04, 2, False, 512, 0)
'Far side

    'Define near and far side hole elements

    'Near side countersink
    Set swAdvHole\_Near\_1 =
swModel.**Extension**.**CreateAdvancedHoleElementData**(swAdvWzdGeneralHoleTypes\_e.swAdvWzdCounterSink)
    swAdvHole\_Near\_1.**Orientation** = swHoleElementOrientation\_e.swHoleElementOrientation\_Nearside
    swAdvHole\_Near\_1.**Size** = "#4"
    swAdvHole\_Near\_1.**Standard** = swWzdHoleStandards\_e.swStandardAnsiInch
    swAdvHole\_Near\_1.**FastenerType** =
swWzdHoleStandardFastenerTypes\_e.swStandardAnsiInchFlatHead100
    swAdvHole\_Near\_1.**Diameter** = ConvFactorLength \* 0.225
    swAdvHole\_Near\_1.**BlindDepth** = 0.02055794 \* ConvFactorLength
    swAdvHole\_Near\_1.**EndCondition** = swEndConditions\_e.swEndCondBlind
    Set swCounterSinkNear = swAdvHole\_Near\_1
    swCounterSinkNear.**EndConditionOverride** = True
    swCounterSinkNear.**AngleOverride** = False

    'Near side straight tap
    Set swAdvHole\_Near\_2 =
swModel.**Extension**.**CreateAdvancedHoleElementData**(swAdvWzdGeneralHoleTypes\_e.swAdvWzdStraightTap)

    swAdvHole\_Near\_2.**Orientation** =
swHoleElementOrientation\_e.swHoleElementOrientation\_Nearside
    swAdvHole\_Near\_2.**Size** = "#4-40"
    swAdvHole\_Near\_2.**Standard** = swWzdHoleStandards\_e.swStandardAnsiInch
    swAdvHole\_Near\_2.**FastenerType** = swWzdHoleStandardFastenerTypes\_e.swStandardAnsiInchBottomingTappedHole
    swAdvHole\_Near\_2.**Diameter** = ConvFactorLength \* 0.089
    swAdvHole\_Near\_2.**EndCondition** = swEndConditions\_e.swEndCondUpToNext
    swAdvHole\_Near\_2.**DiameterOverride** = True
    Set swStraightTapNear = swAdvHole\_Near\_2
    swStraightTapNear.**CustomSizing** =
swStraightTapHoleCustomSizing\_e.swStraightTapHoleCustomSizing\_TapDrillDiameter
    swStraightTapNear.**ThreadClass** =
swStraightTapHoleThreadClass\_e.swStraightTapHoleThreadClass\_1B
    swStraightTapNear.**ThreadClassOverride** = True

    'Near side tapered tap
    Set swAdvHole\_Near\_3 =
swModel.**Extension**.**CreateAdvancedHoleElementData**(swAdvWzdGeneralHoleTypes\_e.swAdvWzdTaperTap)
    swAdvHole\_Near\_3.**Orientation** = swHoleElementOrientation\_e.swHoleElementOrientation\_Nearside
    swAdvHole\_Near\_3.**Size** = "1/16"
    swAdvHole\_Near\_3.**Standard** = swWzdHoleStandards\_e.swStandardAnsiInch
    swAdvHole\_Near\_3.**FastenerType** = swWzdHoleStandardFastenerTypes\_e.swStandardAnsiInchTaperedPipeTap
    swAdvHole\_Near\_3.**Diameter** = ConvFactorLength \* 0.266
    swAdvHole\_Near\_2.**BlindDepth** = 0.205 \* ConvFactorLength
    swAdvHole\_Near\_3.**EndCondition** = swEndConditions\_e.swEndCondBlind
    swAdvHole\_Near\_3.**DiameterOverride** = True
    Set swTaperedTapNear = swAdvHole\_Near\_3
    swTaperedTapNear.**CustomSizing** =
swTaperedTapCustomSizing\_e.swTaperedTapCustomSizing\_MinorDiameterwithCosmeticThread
    swTaperedTapNear.**ThreadClass** =
swTaperedTapThreadClass\_e.swTaperedTapThreadClass\_1
    swTaperedTapNear.**ThreadClassOverride** = True
    swTaperedTapNear.**EndConditionOverride** = True

    'Far side counterbore
    Set swAdvHole\_Far\_1 =
swModel.**Extension**.**CreateAdvancedHoleElementData**(swAdvWzdGeneralHoleTypes\_e.swAdvWzdCounterBore)
    swAdvHole\_Far\_1.**Orientation** = swHoleElementOrientation\_e.swHoleElementOrientation\_Farside
    swAdvHole\_Far\_1.**Size** = "#8"
    swAdvHole\_Far\_1.**Standard** = swWzdHoleStandards\_e.swStandardAnsiInch
    swAdvHole\_Far\_1.**FastenerType** = swWzdHoleStandardFastenerTypes\_e.swStandardAnsiInchBinding
    swAdvHole\_Far\_1.**Diameter** = ConvFactorLength \* 0.375
    swAdvHole\_Far\_1.**BlindDepth** = 0.105 \* ConvFactorLength
    swAdvHole\_Far\_1.**EndCondition** = swEndConditions\_e.swEndCondBlind
    swAdvHole\_Far\_1.**DiameterOverride** = True
    Set swCounterBoreFar = swAdvHole\_Far\_1
    swCounterBoreFar.**EndConditionOverride** = True

    'Far side straight hole
    Set swAdvHole\_Far\_2 =
swModel.**Extension**.**CreateAdvancedHoleElementData**(swAdvWzdGeneralHoleTypes\_e.swAdvWzdStraight)

    swAdvHole\_Far\_2.**Orientation** =
swHoleElementOrientation\_e.swHoleElementOrientation\_Farside
    swAdvHole\_Far\_2.**Size** = "1/16"
    swAdvHole\_Far\_2.**Standard** = swWzdHoleStandards\_e.swStandardAnsiInch
    swAdvHole\_Far\_2.**FastenerType** = swWzdHoleStandardFastenerTypes\_e.swStandardAnsiInchAllDrillSizes
    swAdvHole\_Far\_2.**Diameter** = ConvFactorLength \* 0.0625
    swAdvHole\_Far\_2.**BlindDepth** = 0.2711 \* ConvFactorLength
    swAdvHole\_Far\_2.**EndCondition** = swEndConditions\_e.swEndCondBlind
    swAdvHole\_Far\_2.**DiameterOverride** = True

    'Customize the hole callout for this
straight element
    StrDiam = swModel.**Extension**.**GetCalloutVariableString**(swCalloutVariable\_AH\_Straight\_Diameter)
    strDepth = swModel.**Extension**.**GetCalloutVariableString**(swCalloutVariable\_AH\_Straight\_Depth)
    CalloutString = "<MOD-DIAM> " & StrDiam & " " & "<HOLE-DEPTH>
" & strDepth
    swAdvHole\_Far\_2.**CalloutString** = CalloutString
    Set swStraightHoleFar = swAdvHole\_Far\_2

    'Set the near and far side arrays; stack
ordering is from the near and far side faces
    Set advHoleNearArr(0) = swCounterSinkNear
    Set advHoleNearArr(1) = swStraightTapNear
    Set advHoleFarArr(0) = swCounterBoreFar
    Set advHoleFarArr(1) = swStraightHoleFar

    Set feat =
swFeatureMgr.**AdvancedHole2**((advHoleNearArr), (advHoleFarArr), False, True,
False, ResultArray)

    'Get the near and far side element data
    Set featdata = feat.**GetDefinition**
    featdata.**AccessSelections** swModel, Nothing
    Debug.Print "Number of near side hole elements: " &
featdata.**NearSideElementsCount**
    Debug.Print "Number of far side hole elements: " &
featdata.**FarSideElementsCount**
    Set swCounterSinkNear = featdata.**GetNearSideElements**(0)
    Set swCounterBoreFar = featdata.**GetFarSideElements**(0)
    Debug.Print "Near side countersink:"
    Debug.Print "   Hole element type as defined in
swAdvWzdGeneralHoleTypes\_e: " & swCounterSinkNear.**ElementType**
    Debug.Print "   Size as defined on the Advanced
Hole PropertyManager page: " & swCounterSinkNear.**Size**
    Debug.Print "   Standard as defined in
swWzdHoleStandards\_e: " & swCounterSinkNear.**Standard**
    Debug.Print "   Fastener type as defined in
swWzdHoleStandardFastenerTypes\_e: " & swCounterSinkNear.**FastenerType**
    Debug.Print "   Diameter in m: " &
swCounterSinkNear.**Diameter**
    Debug.Print "   Blind depth in m: " &
swCounterSinkNear.**BlindDepth**
    Debug.Print "   Orientation as defined in
swHoleElementOrientation\_e: " & swCounterSinkNear.**Orientation**
    Debug.Print "   End condition as defined in
swEndConditions\_e: " & swCounterSinkNear.**EndCondition**

    Debug.Print "Far side straight:"
    Debug.Print "   Hole element type as defined in
swAdvWzdGeneralHoleTypes\_e: " & swStraightHoleFar.**ElementType**
    Debug.Print "   Size as defined on the Advanced
Hole PropertyManager page: " & swStraightHoleFar.**Size**
    Debug.Print "   Standard as defined in
swWzdHoleStandards\_e: " & swStraightHoleFar.**Standard**
    Debug.Print "   Fastener type as defined in
swWzdHoleStandardFastenerTypes\_e: " & swStraightHoleFar.**FastenerType**
    Debug.Print "   Diameter in m: " &
swStraightHoleFar.**Diameter**    Debug.Print "   Diameter override? " &
swStraightHoleFar.**DiameterOverride**
    Debug.Print "   Blind depth in m: " &
swStraightHoleFar.**BlindDepth**    Debug.Print "   Orientation as defined in
swHoleElementOrientation\_e: " & swStraightHoleFar.**Orientation**
    Debug.Print "   End condition as defined in
swEndConditions\_e: " & swStraightHoleFar.**EndCondition**
    Debug.Print "   Customized hole callout: " &
swStraightHoleFar.**CalloutString**

    'Modify the near and far side element
arrays
    Set newNearArr(0) = swTaperedTapNear
    Set newNearArr(1) = swStraightTapNear
    'Set newFarArr(0) = swCounterBoreFar
    'Set newFarArr(1) = swStraightHoleFar
    featdata.**SetNearSideElements** newNearArr
    'featdata.**SetFarSideElements** newFarArr
    feat.**ModifyDefinition** featdata, swModel, Nothing

    'Delete the first point used to define the
Advanced Hole
    Set swSketchFeature = feat.**GetFirstSubFeature**
    swSketchFeature.**Select2** False, 0
    swModel.**EditSketch**
    Set swSelectionManager = swModel.**SelectionManager**
    Set swSketch = swSketchFeature.**GetSpecificFeature2**()
    swSketchPointArray = swSketch.**GetSketchPoints2**()
    swMaxPointNumber = UBound(swSketchPointArray)
    For swCurrentPointNumber = 0 To swMaxPointNumber Step 1
       Set swSketchPoint =
swSketchPointArray(swCurrentPointNumber)
       retval =
swSelectionManager.**AddSelectionListObject**(swSketchPoint, Nothing)
       swModel.**EditDelete**
    Next swCurrentPointNumber

    'Create points for multiple Advanced Hole
locations
    Set skPoint = swModel.**SketchManager**.**CreatePoint**(-3.19158789518497E-02,
3.44489966898323E-02, 0.05600000000004)
    Set skPoint = swModel.**SketchManager**.**CreatePoint**(-4.94104502066557E-02,
8.0156770060853E-03, 5.60000000000969E-02)

    swModel.**SketchManager**.**InsertSketch** True

End Sub