<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IMatchedBoolean.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IMatchedBoolean Method (IBody2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : IMatchedBoolean Method (IBody2) |

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

*NumOfMatchingFaces*

*FaceList1*

*FaceList2*

*ErrorCode*

Obsolete. Superseded by [IBody2::IMatchedBoolean3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~IMatchedBoolean3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IMatchedBoolean( _    ByVal OperationType As System.Integer, _    ByVal ToolBody As Body2, _    ByVal NumOfMatchingFaces As System.Integer, _    ByRef FaceList1 As Face2, _    ByRef FaceList2 As Face2, _    ByRef ErrorCode As System.Integer _ ) As EnumBodies2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim OperationType As System.Integer Dim ToolBody As Body2 Dim NumOfMatchingFaces As System.Integer Dim FaceList1 As Face2 Dim FaceList2 As Face2 Dim ErrorCode As System.Integer Dim value As EnumBodies2   value = instance.IMatchedBoolean(OperationType, ToolBody, NumOfMatchingFaces, FaceList1, FaceList2, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` EnumBodies2 IMatchedBoolean(     System.int OperationType,    Body2 ToolBody,    System.int NumOfMatchingFaces,    ref Face2 FaceList1,    ref Face2 FaceList2,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` EnumBodies2^ IMatchedBoolean(  &   System.int OperationType, &   Body2^ ToolBody, &   System.int NumOfMatchingFaces, &   Face2^% FaceList1, &   Face2^% FaceList2, &   [Out] System.int ErrorCode ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*OperationType*

*ToolBody*

*NumOfMatchingFaces*

*FaceList1*

*FaceList2*

*ErrorCode*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::IMatchedBoolean.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)