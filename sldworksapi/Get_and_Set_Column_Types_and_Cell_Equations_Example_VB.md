<!-- source: sldworksapi/Get_and_Set_Column_Types_and_Cell_Equations_Example_VB.htm -->

# SOLIDWORKS API Help

# Get and Set BOM Column Types and Cell Equations Example (VBA)

This example shows how to get and set BOM table column types and cell equations.

'----------------------------------------------------------------------------
' Preconditions:
' 1. Ensure the specified drawing and BOM template exist.
' 2. Open the Immediate window.
'
' Postconditions:
' 1. Opens a document and inserts a BOM table annotation.
' 2. Inserts three rows at the bottom of the table.
' 3. Populates the first three rows of the Description column with
'    10, 20, and 30, respectively.
' 4. Inserts multiple columns of various types.
' 5. Sets equation, SUM(C1:C3), in cell(4,2), gets it, and evaluates it.
' 6. Examine the BOM table and the Immediate window.
'
' NOTE: Because the model is used elsewhere, do not save changes.
'---------------------------------------------------------------------------
Option Explicit

Dim swApp As SldWorks.SldWorks
Dim swModel As SldWorks.ModelDoc2
Dim boolstatus As Boolean
Dim SelMgr As SldWorks.SelectionMgr
Dim theTableAnnotation As SldWorks.TableAnnotation
Dim SelObjType As Long
Dim TableAnnotationType As Long
Dim PropData As Variant
Dim longstatus As Long, longwarnings As Long

Sub main()
    Dim property\_string As String
    Dim cellequation As String
    Dim solvedval As String

    Set swApp = Application.SldWorks
    Set swModel = swApp.**OpenDoc6**("C:\Users\Public\Documents\SOLIDWORKS\SOLIDWORKS
2019\samples\tutorial\advdrawings\foodprocessor.slddrw", 3, 0, "", longstatus,
longwarnings)
    Dim swDrawing As SldWorks.DrawingDoc
    Set swDrawing = swModel
    swApp.**ActivateDoc2** "foodprocessor - Sheet1", False,
longstatus
    Set swModel = swApp.**ActiveDoc**
    boolstatus = swModel.**ActivateView**("Drawing View1")
    Dim swActiveView As SldWorks.View
    Set swActiveView = swModel.**ActiveDrawingView**
    Dim swBOMTableAnno As SldWorks.BomTableAnnotation
    Set swBOMTableAnno = swActiveView.**InsertBomTable4**(False,
0.111517224639408, 0.36564824,
swBOMConfigurationAnchorType\_e.swBOMConfigurationAnchor\_TopLeft,
swBomType\_e.swBomType\_PartsOnly, "Default", "C:\Program Files\SOLIDWORKS
Corp\SOLIDWORKS\lang\english\bom-standard.sldbomtbt", False, 0, False)
    boolstatus = swModel.**EditRebuild3**()

    Set SelMgr = swModel.**SelectionManager**
    boolstatus = swModel.**Extension**.**SelectByID2**("DetailItem174@Sheet1",
"ANNOTATIONTABLES", 0.196194597542634, 0.368489762580645, 0, False, 0, Nothing,
0)
    SelObjType = SelMgr.**GetSelectedObjectType3**(1, -1)

    If SelObjType <> swSelANNOTATIONTABLES
Then
        MsgBox "Select a BOM table in the
drawing before running this example."
        End
    End If

    Set theTableAnnotation = SelMgr.**GetSelectedObject6**(1,
-1)
    TableAnnotationType = theTableAnnotation.**Type**

    If TableAnnotationType <>
swTableAnnotation\_BillOfMaterials Then
        MsgBox "Select a BOM table in the
drawing before running this example."
        End
    End If

    Debug.Print " "
    Debug.Print " --------------------------------"
    Debug.Print "Table BEFORE inserting a column..."
    Debug.Print " "

    ' Display the table before inserting a
column

    DisplayTableColumnProps theTableAnnotation

    ' Insert Custom Property column
    boolstatus = theTableAnnotation.**InsertColumn2**(swTableItemInsertPosition\_Last,
0, "New Col Custom Property", swInsertColumn\_DefaultWidth)
    property\_string = "SW-Comments(Comments)"
    PropData = property\_string
    longstatus = theTableAnnotation.**SetColumnType3**(theTableAnnotation.ColumnCount
- 1, swBomTableColumnType\_CustomProperty, True, PropData)

    ' Insert Unit Of Measure column
    boolstatus = theTableAnnotation.**InsertColumn2**(swTableItemInsertPosition\_Last,
0, "New Col Unit of Measure", swInsertColumn\_DefaultWidth)
    property\_string = "SW-Title(Title)"
    PropData = property\_string
    longstatus = theTableAnnotation.**SetColumnType3**(theTableAnnotation.ColumnCount
- 1, swBomTableColumnType\_UnitOfMeasure, True, PropData)

    ' Insert Equation column
    boolstatus = theTableAnnotation.**InsertColumn2**(swTableItemInsertPosition\_Last,
0, "New Col Equation", swInsertColumn\_DefaultWidth)
    property\_string = "=2+2"
    PropData = property\_string
    longstatus = theTableAnnotation.**SetColumnType3**(theTableAnnotation.ColumnCount
- 1, swBomTableColumnType\_Equation, True, PropData)

    ' Insert Component Reference column
    boolstatus = theTableAnnotation.**InsertColumn2**(swTableItemInsertPosition\_Last,
0, "New Col Component Ref", swInsertColumn\_DefaultWidth)
    Set PropData = Nothing
    longstatus = theTableAnnotation.**SetColumnType3**(theTableAnnotation.ColumnCount
- 1, swBomTableColumnType\_ComponentReference, True, PropData)

    ' Insert Toolbox Property column
    boolstatus = theTableAnnotation.**InsertColumn2**(swTableItemInsertPosition\_Last,
0, "New Col toolbox", swInsertColumn\_DefaultWidth)
    PropData =
swToolBoxPropertyName\_e.swToolBoxPropertyName\_Specification
    longstatus = theTableAnnotation.**SetColumnType3**(theTableAnnotation.ColumnCount
- 1, swBomTableColumnType\_ToolboxProperty, True, PropData)

    ' Insert Cut List Properties column --
only applicable for sheet metal parts
    boolstatus = theTableAnnotation.**InsertColumn2**(swTableItemInsertPosition\_Last,
0, "New Col Cut List property", swInsertColumn\_DefaultWidth)
    property\_string = "Bends"
    PropData = property\_string
    longstatus = theTableAnnotation.**SetColumnType3**(theTableAnnotation.ColumnCount
- 1, swBomTableColumnType\_CutListProperties, True, PropData)

    ' Insert Item Number column
    boolstatus = theTableAnnotation.**InsertColumn2**(swTableItemInsertPosition\_Last,
0, "New Col Item Number", swInsertColumn\_DefaultWidth)
    PropData = Array(2, 3, True, False)
    longstatus = theTableAnnotation.**SetColumnType3**(theTableAnnotation.ColumnCount
- 1, swBomTableColumnType\_ItemNumber, True, PropData)

    ' Insert Part Number column
    boolstatus = theTableAnnotation.**InsertColumn2**(swTableItemInsertPosition\_Last,
0, "New Col Part Number", swInsertColumn\_DefaultWidth)
    PropData = True ' use title summary
    longstatus = theTableAnnotation.**SetColumnType3**(theTableAnnotation.ColumnCount
- 1, swBomTableColumnType\_PartNumber, True, PropData)

    boolstatus = theTableAnnotation.**InsertRow**(4,
0)
    theTableAnnotation.**Text2**(1, 2, True) = 10
    boolstatus = theTableAnnotation.**InsertRow**(4, 0)
    theTableAnnotation.**Text2**(2, 2, True) = 20
    boolstatus = theTableAnnotation.**InsertRow**(4, 0)
    theTableAnnotation.**Text2**(3, 2, True) = 30

    Debug.Print " "
    Debug.Print " --------------------------------"
    Debug.Print "Table AFTER inserting a column..."
    Debug.Print " "

    ' Display table after inserting a column
    DisplayTableColumnProps theTableAnnotation

    ' Set a cell equation
    longstatus = theTableAnnotation.**SetCellEquation**(4, 2,
True, "=SUM(C2:C4)")
    boolstatus = swModel.EditRebuild3()

    ' Get the cell equation
    cellequation = theTableAnnotation.**GetCellEquation**(4,
2, True, solvedval, longstatus)
    Debug.Print " "
    Debug.Print "Equation set in cell(4,2): " & cellequation

    ' Evaluate the cell equation
    longstatus = theTableAnnotation.**EvaluateCellEquation**(4,
2, True, cellequation, solvedval)
    Debug.Print "   Solved value: " & solvedval

End Sub
Sub DisplayTableColumnProps(theTableAnnotation As TableAnnotation)

    Dim ColCount As Long
    Dim i As Long
    Dim ColType As swTableColumnTypes\_e
    Dim ColTitle As String
    Dim status As Long

    Dim property\_string As String
    Dim toolbox\_property As Long
    Dim start As Long
    Dim increment As Long
    Dim order\_balloons As Boolean
    Dim BOM\_items As Boolean
    Dim titlesummary As Boolean

    Debug.Print "Col#"; vbTab; "Type"; vbTab;
"Title"

    ColCount = theTableAnnotation.**ColumnCount**

    For i = 0 To ColCount - 1

        ColType =
theTableAnnotation.**GetColumnType3**(i, True, PropData, status)
        ColTitle = theTableAnnotation.**GetColumnTitle2**(i,
True)

        Debug.Print i;
vbTab; ColType; vbTab; ColTitle; vbTab

        If ColType =
swTableColumnTypes\_e.swBomTableColumnType\_CustomProperty Then

property\_string = PropData
            Debug.Print "
Property Name: " & property\_string

        ElseIf ColType =
swTableColumnTypes\_e.swBomTableColumnType\_UnitOfMeasure Then

property\_string = PropData
            Debug.Print "
Property Name: " & property\_string

        ElseIf ColType =
swTableColumnTypes\_e.swBomTableColumnType\_Equation Then

property\_string = PropData
            Debug.Print "
Equation     : " & property\_string

        ElseIf ColType =
swTableColumnTypes\_e.swBomTableColumnType\_ComponentReference Then
            ' PropData
should be Nothing since a
            ' component
reference column does not contain additional property data
            If PropData
Is Nothing Then

Debug.Print "
NULL Property data"
            End If

        ElseIf ColType =
swTableColumnTypes\_e.swBomTableColumnType\_ToolboxProperty Then

toolbox\_property = PropData
            Debug.Print "
Toolbox Property: " & toolbox\_property

        ElseIf ColType =
swTableColumnTypes\_e.swBomTableColumnType\_CutListProperties Then

property\_string = PropData
            Debug.Print "
Cut List Property: " & property\_string

        ElseIf ColType =
swTableColumnTypes\_e.swBomTableColumnType\_ItemNumber Then
            start =
PropData(0)
            increment =
PropData(1)

order\_balloons = PropData(2)
            BOM\_items =
PropData(3)
            Debug.Print "
Start    : " & start
            Debug.Print "
Increment: " & increment
            Debug.Print "
Order balloons and Bill of Materials to follow assembly order: " &
order\_balloons
            Debug.Print "
Do not change Bill of Materials item numbers: " & BOM\_items

        ElseIf ColType =
swTableColumnTypes\_e.swBomTableColumnType\_PartNumber Then
            titlesummary
= PropData
            Debug.Print "
Use title summary: " & titlesummary

        End If

    Next i
End Sub