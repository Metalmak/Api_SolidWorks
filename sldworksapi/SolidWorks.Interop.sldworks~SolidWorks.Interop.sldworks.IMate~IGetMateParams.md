<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate~IGetMateParams.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetMateParams Method (IMate) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMate Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate.html) : IGetMateParams Method (IMate) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*MateType*

*AlignFlag*

*CanBeFlipped*

Obsolete. Not superseded.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IGetMateParams( _    ByRef MateType As System.Integer, _    ByRef AlignFlag As System.Integer, _    ByRef CanBeFlipped As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMate Dim MateType As System.Integer Dim AlignFlag As System.Integer Dim CanBeFlipped As System.Integer   instance.IGetMateParams(MateType, AlignFlag, CanBeFlipped) ``` | |

| C# |  |
| --- | --- |
| ``` void IGetMateParams(     out System.int MateType,    out System.int AlignFlag,    out System.int CanBeFlipped ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IGetMateParams(  &   [Out] System.int MateType, &   [Out] System.int AlignFlag, &   [Out] System.int CanBeFlipped ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*MateType*

*AlignFlag*

*CanBeFlipped*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Mate::IGetMateParams.

# ![](dotnetimages/collapse.gif)See Also

####

[IMate Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate.html)

[IMate Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate_members.html)