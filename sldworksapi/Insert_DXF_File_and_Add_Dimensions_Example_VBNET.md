<!-- source: sldworksapi/Insert_DXF_File_and_Add_Dimensions_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Insert DXF/DWG File and Add Dimensions Example (VB.NET)

This example shows how to insert a DXF/DWG image on a preselected plane
or face and then autodimension it.

'----------------------------------------------------------------------------
' Preconditions:
' 1. Open a part.
' 2. Replace *path\_name* with the pathname of an existing DXF/DWG file.
' 3. Select a plane or face on which to insert the DXF/DWG image.
'
' Postconditions:
' 1. Adds the DXF/DWG image as a sketch.
' 2. Autodimensions the sketch.
' 3. Use **Zoom to Area** to inspect the sketch dimensioning.
' 4. Press F5 to rebuild the model.
'---------------------------------------------------------------------------
Imports
SolidWorks.Interop.sldworks
Imports
SolidWorks.Interop.swconst
Imports
System

Partial
Class
SolidWorksMacro

    Const
nTolerance As
Double =
0.00000001
    Dim
swModelView As
ModelView
    Dim
swSketchMgr As
SketchManager
    Dim
nRetVal As
Long

    Function
GetAllSketchLines(ByVal
swApp As
SldWorks, ByVal
swModel As
ModelDoc2, ByVal
swSketch As
Sketch) As
Object

        Dim
vSketchSegArr As
Object
        Dim
vSketchSeg As
Object
        Dim
swSketchSeg As
SketchSegment
        Dim
swSketchCurrLine As
SketchLine
        Dim
swSketchLineArr() As
SketchLine
        ReDim
swSketchLineArr(0)

        vSketchSegArr = swSketch.**GetSketchSegments**

        If
Not
IsNothing(vSketchSegArr) Then
            For
Each
vSketchSeg In
vSketchSegArr
                swSketchSeg = vSketchSeg
                If
swSketchSegments\_e.swSketchLINE = swSketchSeg.**GetType**
Then
                    swSketchCurrLine =
swSketchSeg
                    swSketchLineArr(UBound(swSketchLineArr)) =
swSketchCurrLine
                    ReDim
Preserve
swSketchLineArr(UBound(swSketchLineArr) + 1)
                End
If
            Next
        End
If

        If
0 = UBound(swSketchLineArr) Then
            '
No straight lines in this sketch
            GetAllSketchLines =
Nothing
            Exit
Function
        End
If

        '
Remove last, empty sketch line
        ReDim
Preserve
swSketchLineArr(UBound(swSketchLineArr) - 1)
        GetAllSketchLines = swSketchLineArr

    End
Function

    Function
GetSketchPoint(ByVal
swApp As
SldWorks, ByVal
swModel As
ModelDoc2, ByVal
swSketch As
Sketch, ByVal
swSketchPt As
SketchPoint) As
Boolean

        Dim
vSketchPtArr As
Object
        vSketchPtArr =
swSketch.**GetSketchPoints2**
        If
Not
IsNothing(vSketchPtArr) Then
            '
Use first point
            swSketchPt = vSketchPtArr(0)
            GetSketchPoint = True
            Exit
Function
        End
If
        GetSketchPoint =
False

    End
Function

    Function
FindVerticalOrigin(ByVal
swApp As
SldWorks, ByVal
swModel As
ModelDoc2, ByVal
swSketch As
Sketch, ByVal
swSketchSegVert As
SketchSegment, ByVal
swSketchPtVert As
SketchPoint) As
Boolean

        Dim
vSketchLineArr As
Object
        Dim
vSketchLine As
Object
        Dim
swSketchCurrLine As
SketchLine
        Dim
swStartPt As
SketchPoint
        Dim
swEndPt As
SketchPoint

        ' Get first vertical line
        vSketchLineArr =
GetAllSketchLines(swApp, swModel, swSketch)

        If
Not
IsNothing(vSketchLineArr) Then
            For
Each
vSketchLine In
vSketchLineArr
                swSketchCurrLine = vSketchLine
                swStartPt = swSketchCurrLine.**GetStartPoint2**
                swEndPt = swSketchCurrLine.**GetEndPoint2**

                If
Math.Abs(swStartPt.**X** - swEndPt.**X**) < nTolerance
Then
                    swSketchSegVert =
swSketchCurrLine
                    FindVerticalOrigin =
True
                    Exit
Function
                End
If
            Next
        End
If

        '
Get first point
        FindVerticalOrigin =
GetSketchPoint(swApp, swModel, swSketch, swSketchPtVert)

    End
Function

    Function
FindHorizontalOrigin(ByVal
swApp As
SldWorks, ByVal
swModel As
ModelDoc2, ByVal
swSketch As
Sketch, ByVal
swSketchSegHoriz As
SketchSegment, ByVal
swSketchPtHoriz As
SketchPoint) As
Boolean

        Dim
vSketchLineArr As
Object
        Dim
vSketchLine As
Object
        Dim
swSketchCurrLine As
SketchLine
        Dim
swStartPt As
SketchPoint
        Dim
swEndPt As
SketchPoint

        ' Get first horizontal line
        vSketchLineArr =
GetAllSketchLines(swApp, swModel, swSketch)

        If
Not
IsNothing(vSketchLineArr) Then
            For
Each
vSketchLine In
vSketchLineArr
                swSketchCurrLine = vSketchLine
                swStartPt = swSketchCurrLine.**GetStartPoint2**
                swEndPt = swSketchCurrLine.**GetEndPoint2**

                If
Math.Abs(swStartPt.**Y** - swEndPt.**Y**) < nTolerance
Then
                    swSketchSegHoriz =
swSketchCurrLine
                    FindHorizontalOrigin =
True
                    Exit
Function
                End
If
            Next
        End
If

        '
Get first point
        FindHorizontalOrigin =
GetSketchPoint(swApp, swModel, swSketch, swSketchPtHoriz)

    End
Function

    Function
AutoDimensionSketch(ByVal
swApp As
SldWorks, ByVal
swModel As
ModelDoc2, ByVal
swSketch As
Sketch, ByVal
swSelData As
SelectData) As
Long

        Dim
swFeat As
Feature
        Dim
swSketchSegHoriz As
SketchSegment = Nothing
        Dim
swSketchPtHoriz As
SketchPoint = Nothing
        Dim
swSketchSegVert As
SketchSegment = Nothing
        Dim
swSketchPtVert As
SketchPoint = Nothing
        Dim
bRet As
Boolean

        If
False =
FindHorizontalOrigin(swApp, swModel, swSketch, swSketchSegHoriz,
swSketchPtHoriz) Then
            AutoDimensionSketch =
swAutodimStatus\_e.swAutodimStatusDatumLineNotHorizontal
            Exit
Function
        End
If

        If
False =
FindVerticalOrigin(swApp, swModel, swSketch, swSketchSegVert, swSketchPtVert)
Then
            AutoDimensionSketch =
swAutodimStatus\_e.swAutodimStatusDatumLineNotVertical
            Exit
Function
        End
If

        swFeat = swSketch

        bRet = swFeat.**Select2**(False,
0)

        ' Editing sketch clears selections
        swModel.**EditSketch**()
        ' Reselect sketch segments with
correct marks for auto-dimensioning
        If
Not
swSketchSegVert Is
Nothing
Then
            '
Vertical line is for horizontal datum
            bRet = swSketchSegVert.**Select4**(True,
swSelData)
        ElseIf
Not
swSketchPtHoriz Is
Nothing
Then
            bRet = swSketchPtHoriz.**Select4**(True,
swSelData)
        ElseIf
Not
swSketchPtVert Is
Nothing
Then
            '
Use any sketch point for horizontal datum
            bRet = swSketchPtVert.**Select4**(True,
swSelData)
        End
If

        If
Not
swSketchSegHoriz Is
Nothing
Then
            '
Horizontal line is for vertical datum
            bRet =
swSketchSegHoriz.**Select4**(True,
swSelData)
        ElseIf
Not
swSketchPtVert Is
Nothing
Then
            bRet = swSketchPtVert.**Select4**(True,
swSelData)
        ElseIf
Not
swSketchPtHoriz Is
Nothing
Then
            '
Use any sketch point for vertical datum
            bRet = swSketchPtHoriz.**Select4**(True,
swSelData)
        End
If

        '
No straight lines, probably contains circles
        '
so use sketch points for datums
        If
IsNothing(GetAllSketchLines(swApp, swModel, swSketch))
Then
            If
Not
swSketchPtHoriz Is
Nothing
Then
                bRet =
swSketchPtHoriz.**Select4**(False,
swSelData)
            ElseIf
Not
swSketchPtVert Is
Nothing
Then
                bRet =
swSketchPtVert.**Select4**(False,
swSelData)
            End
If
        End
If

        swSketchMgr = swModel.**SketchManager**
        nRetVal = swSketchMgr.**FullyDefineSketch**(True,
True,
swSketchFullyDefineRelationType\_e.swSketchFullyDefineRelationType\_Vertical
Or
swSketchFullyDefineRelationType\_e.swSketchFullyDefineRelationType\_Horizontal,
True, 1,
Nothing, 1,
Nothing, 1,
1)

        ' Redraw so dimensions are
displayed immediately
        Dim
rect() As
Double
        rect =
Nothing
        swModelView.**GraphicsRedraw**(rect)

    End
Function

    Sub
main()

        Const
sDwgFileName As
String =
"*path\_name*"

        Dim
swModel As
ModelDoc2
        Dim
swFeatMgr As
FeatureManager
        Dim
swFeat As
Feature
        Dim
swSketch As
Sketch
        Dim
swSelMgr As
SelectionMgr
        Dim
swSelData As
SelectData
        Dim
bRet As
Boolean
        Dim
importData As
ImportDxfDwgData

        swModel = swApp.**ActiveDoc**
        swModelView = swModel.**ActiveView**
        swFeatMgr = swModel.**FeatureManager**
        importData = swApp.**GetImportFileData**(sDwgFileName)

        'Unit
        importData.**LengthUnit**("")
= swLengthUnit\_e.swMM

        'Position
        bRet = importData.**SetPosition**("",
swDwgImportEntitiesPositioning\_e.swDwgEntitiesCentered, 0, 0)

        'Sheet scale
        bRet = importData.**SetSheetScale**("",
1.0#, 2.0#)

        'Paper size
        bRet = importData.**SetPaperSize**("",
swDwgPaperSizes\_e.swDwgPaperAsize, 0.0#, 0.0#)

        'Import method
        importData.**ImportMethod**("")
= swImportDxfDwg\_ImportMethod\_e.swImportDxfDwg\_ImportToExistingPart

        swFeat = swFeatMgr.**InsertDwgOrDxfFile2**(sDwgFileName,
importData)

        swSketch = swFeat.**GetSpecificFeature2**
        swSelMgr = swModel.**SelectionManager**
        swSelData = swSelMgr.**CreateSelectData**

        nRetVal = AutoDimensionSketch(swApp, swModel, swSketch, swSelData)

        Stop

        '
Rebuild to update sketch
        swModel.**EditRebuild3**()

    End
Sub

    Public
swApp As
SldWorks

End
Class