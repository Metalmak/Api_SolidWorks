<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler~ICheckInterference.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ICheckInterference Method (IModeler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html) : ICheckInterference Method (IModeler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Body1InterferedFaceArray*

*Body2InterferedFaceArray*

*IntersectedBodyArray*

Obsolete. Superseded by [IModeler::ICheckInterference2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModeler~ICheckInterference2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ICheckInterference( _    ByRef Body1InterferedFaceArray As Face, _    ByRef Body2InterferedFaceArray As Face, _    ByRef IntersectedBodyArray As Body _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModeler Dim Body1InterferedFaceArray As Face Dim Body2InterferedFaceArray As Face Dim IntersectedBodyArray As Body   instance.ICheckInterference(Body1InterferedFaceArray, Body2InterferedFaceArray, IntersectedBodyArray) ``` | |

| C# |  |
| --- | --- |
| ``` void ICheckInterference(     out Face Body1InterferedFaceArray,    out Face Body2InterferedFaceArray,    out Body IntersectedBodyArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ICheckInterference(  &   [Out] Face^ Body1InterferedFaceArray, &   [Out] Face^ Body2InterferedFaceArray, &   [Out] Body^ IntersectedBodyArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Body1InterferedFaceArray*

*Body2InterferedFaceArray*

*IntersectedBodyArray*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Modeler::ICheckInterference.

# ![](dotnetimages/collapse.gif)See Also

####

[IModeler Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler.html)

[IModeler Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModeler_members.html)