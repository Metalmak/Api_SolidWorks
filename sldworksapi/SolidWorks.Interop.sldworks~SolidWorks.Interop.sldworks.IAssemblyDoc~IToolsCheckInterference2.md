<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~IToolsCheckInterference2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IToolsCheckInterference2 Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : IToolsCheckInterference2 Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumComponents*

*LpComponents*

*CoincidentInterference*

*PComp*

*PFace*

Obsolete. See [IAssemblyDoc::IToolsCheckInterference3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAssemblyDoc~IToolsCheckInterference3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IToolsCheckInterference2( _    ByVal NumComponents As System.Integer, _    ByRef LpComponents As Component, _    ByVal CoincidentInterference As System.Boolean, _    ByRef PComp As System.Object, _    ByRef PFace As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim NumComponents As System.Integer Dim LpComponents As Component Dim CoincidentInterference As System.Boolean Dim PComp As System.Object Dim PFace As System.Object   instance.IToolsCheckInterference2(NumComponents, LpComponents, CoincidentInterference, PComp, PFace) ``` | |

| C# |  |
| --- | --- |
| ``` void IToolsCheckInterference2(     System.int NumComponents,    ref Component LpComponents,    System.bool CoincidentInterference,    out System.object PComp,    out System.object PFace ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IToolsCheckInterference2(  &   System.int NumComponents, &   Component^% LpComponents, &   System.bool CoincidentInterference, &   [Out] System.Object^ PComp, &   [Out] System.Object^ PFace ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumComponents*

*LpComponents*

*CoincidentInterference*

*PComp*

*PFace*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::IToolsCheckInterference2.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)