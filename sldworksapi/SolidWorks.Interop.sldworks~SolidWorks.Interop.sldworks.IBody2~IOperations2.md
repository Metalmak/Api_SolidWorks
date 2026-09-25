<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~IOperations2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IOperations2 Method (IBody2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : IOperations2 Method (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*OperationType*
:   Operation type as defined in swBodyOperationType\_e

*ToolBody*
:   Pointer to the tool [body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

*ErrorCode*
:   Error indicator as defined in swBodyOperationError\_e; returns swBodyOperationNoError if SOLIDWORKS does not generate an error

Performs add, cut, and intersect (unite, subtract, and interfere) operations between two temporary bodies.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IOperations2( _    ByVal OperationType As System.Integer, _    ByVal ToolBody As Body2, _    ByRef ErrorCode As System.Integer _ ) As EnumBodies2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim OperationType As System.Integer Dim ToolBody As Body2 Dim ErrorCode As System.Integer Dim value As EnumBodies2   value = instance.IOperations2(OperationType, ToolBody, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` EnumBodies2 IOperations2(     System.int OperationType,    Body2 ToolBody,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` EnumBodies2^ IOperations2(  &   System.int OperationType, &   Body2^ ToolBody, &   [Out] System.int ErrorCode ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*OperationType*
:   Operation type as defined in swBodyOperationType\_e

*ToolBody*
:   Pointer to the tool [body](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2.html)

*ErrorCode*
:   Error indicator as defined in swBodyOperationError\_e; returns swBodyOperationNoError if SOLIDWORKS does not generate an error

#### Return Value

Resulting [bodies enumeration](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEnumBodies2.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Body2::IOperations2.

# ![](dotnetimages/collapse.gif)Remarks

If the target and tool bodies are the same in geometry, the result body of this method is NULL, and the return value is S\_false.

This method works with two temporary bodies; one is the target and one is the tool. The output is a list of bodies resulting from the operation.

The two temporary bodies used in this function (the Body2 and ToolBody pointers) are invalid once the operation is complete. COM applications should release these two pointers after using this method. If your application needs to maintain these bodies, then you should make a copy of them using [IBody2::ICopy](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~ICopy.html) before passing them to this routine.

To perform a swBodyOperationType\_e.SWBODYINTERSECT between a sheet (surface) and a solid body, the sheet body must be the target body.

Use [IBody2::Check3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~Check3.html) for both bodies before using this method to ensure that both bodies are valid solids. Using this method with invalid bodies can cause unexpected results.

If a non-manifold error is returned, use [IBody2::ResetEdgeTolerances](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~ResetEdgeTolerances.html) to visit all of the edges in the body to reset their tolerances. Then use IBody2::Operations2 again.

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

[IBody2::Operations2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Operations2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0