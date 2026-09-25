<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody~IOperations.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IOperations Method (IBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html) : IOperations Method (IBody) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*OperationType*

*ToolBody*

*NumMaxSections*

*ResultingBodies*

Obsolete. Superseded by [IBody2::IOperations2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~IOperations2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IOperations( _    ByVal OperationType As System.Integer, _    ByVal ToolBody As Body, _    ByVal NumMaxSections As System.Integer, _    ByRef ResultingBodies As Body _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody Dim OperationType As System.Integer Dim ToolBody As Body Dim NumMaxSections As System.Integer Dim ResultingBodies As Body Dim value As System.Integer   value = instance.IOperations(OperationType, ToolBody, NumMaxSections, ResultingBodies) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IOperations(     System.int OperationType,    Body ToolBody,    System.int NumMaxSections,    ref Body ResultingBodies ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IOperations(  &   System.int OperationType, &   Body^ ToolBody, &   System.int NumMaxSections, &   Body^% ResultingBodies ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*OperationType*

*ToolBody*

*NumMaxSections*

*ResultingBodies*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body::IOperations.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html)

[IBody Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody_members.html)