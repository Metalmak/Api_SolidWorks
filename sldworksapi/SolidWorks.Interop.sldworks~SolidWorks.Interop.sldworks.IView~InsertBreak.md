<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~InsertBreak.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertBreak Method (IView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : InsertBreak Method (IView) |

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
:   Cut style as defined in swBreakLineStyle\_e

Obsolete. Superseded by [IView::InsertBreak2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~InsertBreak2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertBreak( _    ByVal Orientation As System.Integer, _    ByVal Position1 As System.Double, _    ByVal Position2 As System.Double, _    ByVal Style As System.Integer _ ) As BreakLine ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim Orientation As System.Integer Dim Position1 As System.Double Dim Position2 As System.Double Dim Style As System.Integer Dim value As BreakLine   value = instance.InsertBreak(Orientation, Position1, Position2, Style) ``` | |

| C# |  |
| --- | --- |
| ``` BreakLine InsertBreak(     System.int Orientation,    System.double Position1,    System.double Position2,    System.int Style ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` BreakLine^ InsertBreak(  &   System.int Orientation, &   System.double Position1, &   System.double Position2, &   System.int Style ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Orientation*
:   Horizontal or vertical cut as defined in swBreakLineOrientation\_e

*Position1*
:   Location of the first line in the break (see Remarks)

*Position2*
:   Location of the second line in the break (see Remarks)

*Style*
:   Cut style as defined in swBreakLineStyle\_e

#### Return Value

[Break line](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBreakLine.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::InsertBreak.

# ![](dotnetimages/collapse.gif)Remarks

A break in a drawing view consists of a pair of lines. This method inserts the break lines at the locations indicated by Position1 and Position2.

| **If the orientation of the break is...** | **Then Position1 and Position2 are...** |
| --- | --- |
| Horizontal | Y values, relative to the drawing view origin, indicating where along the Y axis to place the breaks |
| Vertical | X values, relative to the drawing view origin, indicating where along the X axis to place the breaks |

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::GetBreakLineCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetBreakLineCount.html)

[IView::GetBreakLineInfo Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetBreakLineInfo.html)

[IView::GetBreakLines Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetBreakLines.html)

[IView::IGetBreakLineInfo Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetBreakLineInfo.html)

[IView::IGetBreakLines Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetBreakLines.html)

[IView::BreakLineGap Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~BreakLineGap.html)

[IView::IsBroken Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IsBroken.html)

[IDrawingDoc::BreakView Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrawingDoc~BreakView.html)

[IBreakLine::Style Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBreakLine~Style.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0