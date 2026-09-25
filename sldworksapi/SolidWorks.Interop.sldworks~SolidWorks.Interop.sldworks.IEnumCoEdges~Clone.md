<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumCoEdges~Clone.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| Clone Method (IEnumCoEdges) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IEnumCoEdges Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumCoEdges.html) : Clone Method (IEnumCoEdges) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Ppenum*
:   Pointer to the cloned [coedges enumeration](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEnumCoEdges.html)

Clones the a coedges enumeration.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub Clone( _    ByRef Ppenum As EnumCoEdges _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEnumCoEdges Dim Ppenum As EnumCoEdges   instance.Clone(Ppenum) ``` | |

| C# |  |
| --- | --- |
| ``` void Clone(     out EnumCoEdges Ppenum ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Clone(  &   [Out] EnumCoEdges^ Ppenum ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Ppenum*
:   Pointer to the cloned [coedges enumeration](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEnumCoEdges.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EnumCoEdges::Clone.

# ![](dotnetimages/collapse.gif)Remarks

For use in in-process DLLs only.

# ![](dotnetimages/collapse.gif)See Also

####

[IEnumCoEdges Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumCoEdges.html)

[IEnumCoEdges Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumCoEdges_members.html)