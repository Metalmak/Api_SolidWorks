<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector~GetEdgeList.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetEdgeList Method (ICWEdgeWeldConnector) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWEdgeWeldConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector.html) : GetEdgeList Method (ICWEdgeWeldConnector) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ErrorCode*
:   Error code as defined in [swsWeldResultErrorCode\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsWeldResultErrorCode_e.html)

Gets the array of intersecting edges in this edge weld connector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetEdgeList( _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWEdgeWeldConnector Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetEdgeList(ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetEdgeList(     out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetEdgeList(  &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*ErrorCode*
:   Error code as defined in [swsWeldResultErrorCode\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsWeldResultErrorCode_e.html)

#### Return Value

Array of intersecting edges

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWEdgeWeldConnector::GetEdgeList.

# ![](dotnetimages/collapse.gif)Example

See the [ICWEdgeWeldConnector](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method returns the edges that are between corresponding faces of the arrays returned by [ICWEdgeWeldConnector::GetFirstFace](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWEdgeWeldConnector~GetFirstFace.html) and [ICWEdgeWeldConnector::GetSecondFace](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWEdgeWeldConnector~GetSecondFace.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICWEdgeWeldConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector.html)

[ICWEdgeWeldConnector Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector_members.html)

[ICWEdgeWeldConnector::AddEdges Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector~AddEdges.html)

[ICWEdgeWeldConnector::RemoveEdges Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector~RemoveEdges.html)

[ICWEdgeWeldConnector::ReplaceFacesAndEdges Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector~ReplaceFacesAndEdges.html)

[ICWEdgeWeldConnector::ReplaceFacesThenAutoGenerateTouchingEdges Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector~ReplaceFacesThenAutoGenerateTouchingEdges.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0