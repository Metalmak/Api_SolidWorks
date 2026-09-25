<!-- source: swdimxpertapi/Get_DimXpert_Display_Dimensions_and_Feature_Example_VB.htm -->

# SOLIDWORKS API Help

# Get DimXpert Display Dimensions and Feature Example (VBA)

This example shows how to find out if an annotation is a DimXpert display
dimension, and, if so, how to get its DimXpert feature.

'---------------------------------------------------------------------------

' Preconditions:

'  1.
Ensure that the SOLIDWORKS DimXpert type library is

'     loaded
in Tools > References in the
IDE.

'  2. Open
*public\_documents*\samples\tutorial\api\plate\_tolstatus.sldprt.

'  3.
Click View > Toolbars > DimXpert.

'  4.
Click Auto Dimension Scheme
on the
DimXpert toolbar.

'  5.
Make sure Chamfer is selected
in Feature Filters

'     on
the Auto Dimension Scheme PropertyManager page, then click the checkmark

'     to
close the page.

'

' Postconditions: Adds DimXpert display dimensions
to the model.

'

' NOTE: Because this part document is used elsewhere, do not
save changes.

'----------------------------------------------------------------------------

Option Explicit

Dim swApp As SldWorks.SldWorks

Dim swPart As SldWorks.ModelDoc2

Dim swAnnotation As SldWorks.Annotation

Dim swDisplayDimension As SldWorks.DisplayDimension

Sub main()

    Set
swApp = Application.SldWorks

    Set
swPart = swApp.ActiveDoc

    Set
swAnnotation = swPart.GetFirstAnnotation2

    Do
While (Not (swAnnotation Is Nothing))

        Debug.Print
" "

        Debug.Print
"Annotation name = " & swAnnotation.GetName

            If
swAnnotationType\_e.swDisplayDimension = swAnnotation.GetType
Then

                Debug.Print
"  Is
a display dimension? True"

                Set
swDisplayDimension = swAnnotation.GetSpecificAnnotation

                Select
Case (swDisplayDimension.Type2)

                   Case
swDimensionType\_e.swOrdinateDimension

                       Debug.Print
"  Display
dimension type = base ordinate and its subordinates"

                   Case
swDimensionType\_e.swLinearDimension

                       Debug.Print
"  Display
dimension type = linear"

                   Case
swDimensionType\_e.swAngularDimension

                       Debug.Print
"  Display
dimension type  =
angular"

                   Case
swDimensionType\_e.swArcLengthDimension

                       Debug.Print
"  Display
dimension type = arc length"

                   Case
swDimensionType\_e.swRadialDimension

                       Debug.Print
"  Display
dimension type = radial"

                   Case
swDimensionType\_e.swDiameterDimension

                       Debug.Print
"  Display
dimension type = diameter"

                   Case
swDimensionType\_e.swHorOrdinateDimension

                       Debug.Print
"  Display
dimension type = horizontal ordinate"

                   Case
swDimensionType\_e.swVertOrdinateDimension

                       Debug.Print
"  Display
dimension type = vertical ordinate"

                   Case
swDimensionType\_e.swZAxisDimension

                       Debug.Print
"  Display
dimension type = z-axis"

                   Case
swDimensionType\_e.swChamferDimension

                       Debug.Print
"  Display
dimension type = chamfer dimension"

                   Case
swDimensionType\_e.swHorLinearDimension

                       Debug.Print
"  Display
dimension type = horizonal linear"

                   Case
swDimensionType\_e.swVertLinearDimension

                       Debug.Print
"  Display
dimension type = vertical linear"

                   Case
swDimensionType\_e.swScalarDimension

                       Debug.Print
"  Display
dimension type = scalar"

                   Case
Else

                       Debug.Print
"  Display
dimension type = unknown"

                End
Select

                Debug.Print
"  Is
a DimXpert display dimension? " & IIf(swDisplayDimension.IsDimXpert = False, "False",
"True")

                If
swAnnotation.IsDimXpert Then

                    Dim
DimXpertFeat As SwDimXpert.DimXpertFeature

                    Dim
FeatName As String

                    Set
DimXpertFeat = swAnnotation.GetDimXpertFeature()

                    If
Not DimXpertFeat Is Nothing Then

                        FeatName
= DimXpertFeat.Name

                        Debug.Print
"  DimXpert
feature name = " & FeatName

                        Select
Case (DimXpertFeat.Type)

                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_Plane

                                Debug.Print
"  DimXpert
feature type = plane"

                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_Cylinder

                                Debug.Print
"  DimXpert
feature type = cylinder"

                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_Cone

                                Debug.Print
"  DimXpert
feature type = cone"

                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_Extrude

                                Debug.Print
"  DimXpert
feature type =extrude"

                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_Fillet

                                Debug.Print
"  DimXpert
feature type = fillet"

                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_Chamfer

                                Debug.Print
"  DimXpert
feature type = chamfer"

                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_CompoundHole

                                Debug.Print
"  DimXpert
feature type = compound hole"

                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_CompoundWidth

                                Debug.Print
"  DimXpert
feature type = compound width"

                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_CompoundNotch

                                Debug.Print
"  DimXpert
feature type = compound notch"

                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_CompoundClosedSlot3D

                                Debug.Print
"  DimXpert
feature type = compound closed-slot 3D"

                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_IntersectPoint

                                Debug.Print
"  DimXpert
feature type = intersect point"

                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_IntersectLine

                                Debug.Print
"  DimXpert
feature type = intersect line"

                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_IntersectCircle

                                Debug.Print
"  DimXpert
feature type = intersect circle"

                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_IntersectPlane

                                Debug.Print
"  DimXpert
feature type = intersect plane"

                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_Pattern

                                Debug.Print
"  DimXpert
feature type = pattern"

                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_Sphere

                                Debug.Print
"  DimXpert
feature type = sphere"

                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_BestfitPlane

                                Debug.Print
"  DimXpert
feature type = best-fit plane"

                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_Surface

                                Debug.Print
"  DimXpert
feature type = surface"

                            Case
Else

                                Debug.Print
"  DimXpert
feature type = unknown"

                        End
Select

                    End
If

                End
If

                Else

                    Debug.Print
"  Not
a display dimension"

                End
If

            Set
swAnnotation = swAnnotation.GetNext3

    Loop

End Sub