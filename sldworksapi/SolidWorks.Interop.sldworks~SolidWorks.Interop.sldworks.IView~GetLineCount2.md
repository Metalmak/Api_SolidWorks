<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetLineCount2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetLineCount2 Method (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : GetLineCount2 Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*CrossHatchOption*
:   Crosshatch option as defined in swCrossHatchFilter\_e

Gets the number of lines in this view with an option to include or exclude crosshatch lines.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetLineCount2( _    ByVal CrossHatchOption As System.Short _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim CrossHatchOption As System.Short Dim value As System.Integer   value = instance.GetLineCount2(CrossHatchOption) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetLineCount2(     System.short CrossHatchOption ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetLineCount2(  &   System.short CrossHatchOption ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*CrossHatchOption*
:   Crosshatch option as defined in swCrossHatchFilter\_e

#### Return Value

Number of lines

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::GetLineCount2.

# ![](dotnetimages/collapse.gif)Example

[Get Polylines Information (VBA)](Get_Polylines_Information_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call this method before calling [IView::IGetLines4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~IGetLines4.html) to get the size of the array for that method.

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::GetLines4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetLines4.html)

[IView::IGetLines4 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetLines4.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0