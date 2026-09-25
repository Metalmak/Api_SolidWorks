<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge~IsTolerant.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IsTolerant Method (IEdge) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IEdge Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html) : IsTolerant Method (IEdge) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Tolerance*
:   Edge tolerance or gap in meters

Gets whether an edge is tolerant and its tolerance value.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IsTolerant( _    ByRef Tolerance As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEdge Dim Tolerance As System.Double Dim value As System.Boolean   value = instance.IsTolerant(Tolerance) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IsTolerant(     out System.double Tolerance ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IsTolerant(  &   [Out] System.double Tolerance ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Tolerance*
:   Edge tolerance or gap in meters

#### Return Value

True if tolerant, false if not tolerant

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Edge::IsTolerant

# ![](dotnetimages/collapse.gif)Example

[Get Maximum Edge and Vertex Gaps (VBA)](Get_Maximum_Edge_and_Vertex_Gaps_Example_VB.htm)

[Get Maximum Edge and Vertex Gaps (VB.NET)](Get_Maximum_Edge_and_Vertex_Gaps_Example_VBNET.htm)

[Get Maximum Edge and Vertex Gaps (C#)](Get_Maximum_Edge_and_Vertex_Gaps_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If the tolerance (or gap) between common edges in a part:

* is greater than 1/2 of the session precision (i.e., > 5.0E-9 mm), then each edge is tolerant, and this method returns true.* is less than or equal to 1/2 of the session precision (i.e., <= 5.0E-9 mm), then each edge is exact and not tolerant, and this method returns false.

Traverse part body edges and use this method to find the maximum edge gap (tolerance) in a part, which can also be found using the **Tools > Check** dialog in the SOLIDWORKS user interface.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdge Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge.html)

[IEdge Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEdge_members.html)

[IVertex::IsTolerant](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IVertex~IsTolerant.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 SP2, Revision Number 17.2