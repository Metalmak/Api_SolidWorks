<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace~RemoveInnerLoops.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| RemoveInnerLoops Method (IFace) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFace Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace.html) : RemoveInnerLoops Method (IFace) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumOfLoops*

*InnerLoopsIn*

Obsolete. Superseded by [IFace2::RemoveInnterLoops](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~RemoveInnerLoops.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RemoveInnerLoops( _    ByVal NumOfLoops As System.Integer, _    ByVal InnerLoopsIn As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFace Dim NumOfLoops As System.Integer Dim InnerLoopsIn As System.Object Dim value As System.Object   value = instance.RemoveInnerLoops(NumOfLoops, InnerLoopsIn) ``` | |

| C# |  |
| --- | --- |
| ``` System.object RemoveInnerLoops(     System.int NumOfLoops,    System.object InnerLoopsIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ RemoveInnerLoops(  &   System.int NumOfLoops, &   System.Object^ InnerLoopsIn ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumOfLoops*

*InnerLoopsIn*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Face::RemoveInnerLoops.

# ![](dotnetimages/collapse.gif)See Also

####

[IFace Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace.html)

[IFace Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace_members.html)