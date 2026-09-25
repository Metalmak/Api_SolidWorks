<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetDowelSymbols.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetDowelSymbols Method (IView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html) : GetDowelSymbols Method (IView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets all of the dowel symbols on this drawing view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetDowelSymbols() As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IView Dim value As System.Object   value = instance.GetDowelSymbols() ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetDowelSymbols() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetDowelSymbols(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Array of [dowel symbols](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDowelSymbol.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See View::GetDowelSymbols.

# ![](dotnetimages/collapse.gif)Example

[Get Annotations Arrays (VBA)](Get_Annotations_Array_Example_VB.htm)

[Get Annotations Arrays (VB.NET)](Get_Annotations_Arrays_Example_VBNET.htm)

[Get Annotations Arrays (C#)](Get_Annotations_Arrays_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Use this method to obtain the array of dowel symbols all at once instead of calling [IView::GetFirstDowelSymbol](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IView~GetFirstDowelSymbol.html) and then repeatedly calling [IDowelSymbol::GetNext](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDowelSymbol~GetNext.html) to obtain the remaining dowel symbols on this drawing view.

# ![](dotnetimages/collapse.gif)See Also

####

[IView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView.html)

[IView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView_members.html)

[IView::GetDowelSymbolCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~GetDowelSymbolCount.html)

[IView::IGetDowelSymbols Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IView~IGetDowelSymbols.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 SP1, Revision Number 17.1