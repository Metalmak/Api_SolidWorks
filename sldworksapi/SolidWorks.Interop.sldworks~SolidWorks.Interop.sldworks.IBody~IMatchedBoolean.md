<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody~IMatchedBoolean.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IMatchedBoolean Method (IBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html) : IMatchedBoolean Method (IBody) |

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
| ``` Function IMatchedBoolean( _    ByVal OperationType As System.Integer, _    ByVal ToolBody As Body, _    ByVal NumOfMatchingFaces As System.Integer, _    ByRef FaceList1 As Face, _    ByRef FaceList2 As Face, _    ByRef ErrorCode As System.Integer _ ) As EnumBodies ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody Dim OperationType As System.Integer Dim ToolBody As Body Dim NumOfMatchingFaces As System.Integer Dim FaceList1 As Face Dim FaceList2 As Face Dim ErrorCode As System.Integer Dim value As EnumBodies   value = instance.IMatchedBoolean(OperationType, ToolBody, NumOfMatchingFaces, FaceList1, FaceList2, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` EnumBodies IMatchedBoolean(     System.int OperationType,    Body ToolBody,    System.int NumOfMatchingFaces,    ref Face FaceList1,    ref Face FaceList2,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` EnumBodies^ IMatchedBoolean(  &   System.int OperationType, &   Body^ ToolBody, &   System.int NumOfMatchingFaces, &   Face^% FaceList1, &   Face^% FaceList2, &   [Out] System.int ErrorCode ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*OperationType*

*ToolBody*

*NumOfMatchingFaces*

*FaceList1*

*FaceList2*

*ErrorCode*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body::IMatchedBoolean.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody.html)

[IBody Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody_members.html)