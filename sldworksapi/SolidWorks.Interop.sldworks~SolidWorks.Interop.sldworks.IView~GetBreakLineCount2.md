<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetBreakLineCount2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetBreakLineCount2 Method (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : GetBreakLineCount2 Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Size*
:   Size of an array of doubles to allocate in [IView::GetBreakLineInfo2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetBreakLineInfo2.html) and [IView::IGetBreakLineInfo2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~IGetBreakLineInfo2.html)

Gets the number of breaks lines and breaks in this view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetBreakLineCount2( _    ByRef Size As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim Size As System.Integer Dim value As System.Integer   value = instance.GetBreakLineCount2(Size) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetBreakLineCount2(     out System.int Size ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetBreakLineCount2(  &   [Out] System.int Size ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Size*
:   Size of an array of doubles to allocate in [IView::GetBreakLineInfo2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetBreakLineInfo2.html) and [IView::IGetBreakLineInfo2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~IGetBreakLineInfo2.html)

#### Return Value

Number of breaks

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::GetBreakLineCount2.

# ![](dotnetimages/collapse.gif)Example

[Get Break Line Data (VBA)](Get_Break_Line_Data_Example_VB.htm)

[Get Break Line Data (VB.NET)](Get_Break_Line_Data_Example_VBNET.htm)

[Get Break Line Data (C#)](Get_Break_Line_Data_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

A drawing view can have break lines without the break being applied. To determine whether a view is broken, use [IView::IsBroken](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~IsBroken.html).

A break in a drawing view consists of a pair of lines. This method returns the number of breaks in the view. For example, this method returns 3 for a view that has three breaks in it, even though there are six lines on the display.

Call this method before calling [IView::IGetBreakLines](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~IGetBreakLines.html) to determine the size of the array for that method.

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::GetBreakLines Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetBreakLines.html)

[IView::BreakLineGap Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~BreakLineGap.html)

[IView::InsertBreak Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~InsertBreak.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0