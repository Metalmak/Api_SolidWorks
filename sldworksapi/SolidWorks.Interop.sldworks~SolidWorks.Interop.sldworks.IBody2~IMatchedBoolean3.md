<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IMatchedBoolean3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IMatchedBoolean3 Method (IBody2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : IMatchedBoolean3 Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*OperationType*
:   One of these operation types:

    * SWBODYADD

      * SWBODYCUT

        * SWCODYINTERSECT

*ToolBodyCount*
:   Number of bodies

*ToolBodyArr*
:   Array of bodies of size ToolBodyCount

*NumOfMatchingFaces*
:   Number of matching faces

*FaceList1*
:   First face list (see **Remarks**)

*FaceList2*
:   Second face list  (see Remarks)

*ErrorCode*
:   Error indicated as defined inswBodyOperationError\_e

Obsolete. Superseded by [IBody2::IMatchedBoolean4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~IMatchedBoolean4.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IMatchedBoolean3( _    ByVal OperationType As System.Integer, _    ByVal ToolBodyCount As System.Integer, _    ByRef ToolBodyArr As Body2, _    ByVal NumOfMatchingFaces As System.Integer, _    ByRef FaceList1 As Face2, _    ByRef FaceList2 As Face2, _    ByRef ErrorCode As System.Integer _ ) As EnumBodies2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim OperationType As System.Integer Dim ToolBodyCount As System.Integer Dim ToolBodyArr As Body2 Dim NumOfMatchingFaces As System.Integer Dim FaceList1 As Face2 Dim FaceList2 As Face2 Dim ErrorCode As System.Integer Dim value As EnumBodies2   value = instance.IMatchedBoolean3(OperationType, ToolBodyCount, ToolBodyArr, NumOfMatchingFaces, FaceList1, FaceList2, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` EnumBodies2 IMatchedBoolean3(     System.int OperationType,    System.int ToolBodyCount,    ref Body2 ToolBodyArr,    System.int NumOfMatchingFaces,    ref Face2 FaceList1,    ref Face2 FaceList2,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` EnumBodies2^ IMatchedBoolean3(  &   System.int OperationType, &   System.int ToolBodyCount, &   Body2^% ToolBodyArr, &   System.int NumOfMatchingFaces, &   Face2^% FaceList1, &   Face2^% FaceList2, &   [Out] System.int ErrorCode ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*OperationType*
:   One of these operation types:

    * SWBODYADD

      * SWBODYCUT

        * SWCODYINTERSECT

*ToolBodyCount*
:   Number of bodies

*ToolBodyArr*
:   Array of bodies of size ToolBodyCount

*NumOfMatchingFaces*
:   Number of matching faces

*FaceList1*
:   First face list (see **Remarks**)

*FaceList2*
:   Second face list  (see Remarks)

*ErrorCode*
:   Error indicated as defined inswBodyOperationError\_e

#### Return Value

Pointer to the [IEnumBodies2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEnumBodies2.html) object for a list of matches

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::IMatchedBoolean3.

# ![](dotnetimages/collapse.gif)Remarks

The concept of match means that the caller tells the boolean operator beforehand which faces can be considered to coincide. Basically, the caller performs part of the boolean operation.

Sometimes the application knows that two faces match because of the way the bodies are constructed; i.e., the application knows which faces are intended to match.

Having a list of matching face pairs may allow the matched boolean operator to resolve other geometric operations that otherwise it would not be able to work out. In general, providing matched faces speeds up the boolean operation and makes results more reliable.

The arguments FaceList1 and FaceList2 arguments can be empty lists. If matching face pairs are passed in, these faces must match such that:

* the surface geometry is coinciding.

  * for each edge in a face, there is an edge in the other face that coincides

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

[IBody2::MatchedBoolean3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~MatchedBoolean3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0