<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate~IGetMateEntities.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetMateEntities Method (IMate) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMate Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate.html) : IGetMateEntities Method (IMate) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Entity1*

*Entity2*

Obsolete. Not superseded.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IGetMateEntities( _    ByRef Entity1 As MateEntity, _    ByRef Entity2 As MateEntity _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMate Dim Entity1 As MateEntity Dim Entity2 As MateEntity   instance.IGetMateEntities(Entity1, Entity2) ``` | |

| C# |  |
| --- | --- |
| ``` void IGetMateEntities(     out MateEntity Entity1,    out MateEntity Entity2 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IGetMateEntities(  &   [Out] MateEntity^ Entity1, &   [Out] MateEntity^ Entity2 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Entity1*

*Entity2*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Mate::IGetMateEntities.

# ![](dotnetimages/collapse.gif)See Also

####

[IMate Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate.html)

[IMate Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate_members.html)