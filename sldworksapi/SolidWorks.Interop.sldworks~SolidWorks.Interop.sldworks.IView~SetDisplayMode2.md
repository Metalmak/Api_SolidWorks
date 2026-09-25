<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~SetDisplayMode2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetDisplayMode2 Method (IView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : SetDisplayMode2 Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Mode*

*Facetted*

*Edges*

Obsolete. Superseded by [IView::SetDisplayMode3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~SetDisplayMode3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetDisplayMode2( _    ByVal Mode As System.Integer, _    ByVal Facetted As System.Boolean, _    ByVal Edges As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim Mode As System.Integer Dim Facetted As System.Boolean Dim Edges As System.Boolean Dim value As System.Boolean   value = instance.SetDisplayMode2(Mode, Facetted, Edges) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetDisplayMode2(     System.int Mode,    System.bool Facetted,    System.bool Edges ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetDisplayMode2(  &   System.int Mode, &   System.bool Facetted, &   System.bool Edges ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Mode*

*Facetted*

*Edges*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::SetDisplayMode2.

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)