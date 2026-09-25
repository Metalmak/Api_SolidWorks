<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~InsertBreak3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertBreak3 Method (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : InsertBreak3 Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Orientation*
:   Horizontal or vertical cut as defined in swBreakLineOrientation\_e

*Position1*
:   Location of the first line in the break (see Remarks)

*Position2*
:   Location of the second line in the break (see Remarks)

*Style*
:   Break line style as defined in swBreakLineStyle\_e

*ShapeIntensity*
:   Shape intensity for jagged cut break lines only; valid range is 1 (most) through 5 (least)

*BreakSketchBlocks*
:   True to break sketch blocks, false to not

Inserts the specified type of break at the specified location in this drawing view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertBreak3( _    ByVal Orientation As System.Integer, _    ByVal Position1 As System.Double, _    ByVal Position2 As System.Double, _    ByVal Style As System.Integer, _    ByVal ShapeIntensity As System.Integer, _    ByVal BreakSketchBlocks As System.Boolean _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim Orientation As System.Integer Dim Position1 As System.Double Dim Position2 As System.Double Dim Style As System.Integer Dim ShapeIntensity As System.Integer Dim BreakSketchBlocks As System.Boolean Dim value As System.Object   value = instance.InsertBreak3(Orientation, Position1, Position2, Style, ShapeIntensity, BreakSketchBlocks) ``` | |

| C# |  |
| --- | --- |
| ``` System.object InsertBreak3(     System.int Orientation,    System.double Position1,    System.double Position2,    System.int Style,    System.int ShapeIntensity,    System.bool BreakSketchBlocks ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ InsertBreak3(  &   System.int Orientation, &   System.double Position1, &   System.double Position2, &   System.int Style, &   System.int ShapeIntensity, &   System.bool BreakSketchBlocks ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Orientation*
:   Horizontal or vertical cut as defined in swBreakLineOrientation\_e

*Position1*
:   Location of the first line in the break (see Remarks)

*Position2*
:   Location of the second line in the break (see Remarks)

*Style*
:   Break line style as defined in swBreakLineStyle\_e

*ShapeIntensity*
:   Shape intensity for jagged cut break lines only; valid range is 1 (most) through 5 (least)

*BreakSketchBlocks*
:   True to break sketch blocks, false to not

#### Return Value

[Break line](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakLine.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::InsertBreak3.

# ![](dotnetimages/collapse.gif)Example

[Insert Jagged Cut Break (VBA)](Insert_Jagged_Cut_Break_Example_VB.htm)

[Insert Jagged Cut Break (VB.NET)](Insert_Jagged_Cut_Break_Example_VBNET.htm)

[Insert Jagged Cut Break (C#)](Insert_Jagged_Cut_Break_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

A break in a drawing view consists of a pair of break lines. This method inserts the break lines at the locations indicated by Position1 and Position2.

| If the orientation of the break is... | Then Position1 and Position2 are... |
| --- | --- |
| Horizontal | Y values relative to the drawing view origin, indicating where along the Y axis to place the breaks |
| Vertical | X values relative to the drawing view origin, indicating where along the X axis to place the breaks |

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::GetBreakLineCount2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetBreakLineCount2.html)

[IView::GetBreakLineInfo2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetBreakLineInfo2.html)

[IView::GetBreakLines Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetBreakLines.html)

[IView::IsBroken Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IsBroken.html)

[IView::BreakLineGap Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~BreakLineGap.html)

[IDrawingDoc::BreakView Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~BreakView.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0