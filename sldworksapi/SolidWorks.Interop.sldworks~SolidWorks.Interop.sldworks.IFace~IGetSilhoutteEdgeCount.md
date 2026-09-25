<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace~IGetSilhoutteEdgeCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetSilhoutteEdgeCount Method (IFace) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFace Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace.html) : IGetSilhoutteEdgeCount Method (IFace) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Root*

*Normal*

Obsolete. Superseded by [IFace2::IGetSilhoutteEdgeCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~IGetSilhoutteEdgeCount.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetSilhoutteEdgeCount( _    ByRef Root As System.Double, _    ByRef Normal As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFace Dim Root As System.Double Dim Normal As System.Double Dim value As System.Integer   value = instance.IGetSilhoutteEdgeCount(Root, Normal) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IGetSilhoutteEdgeCount(     ref System.double Root,    ref System.double Normal ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IGetSilhoutteEdgeCount(  &   System.double% Root, &   System.double% Normal ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Root*

*Normal*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Face::IGetSilhoutteEdgeCount.

# ![](dotnetimages/collapse.gif)See Also

####

[IFace Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace.html)

[IFace Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace_members.html)