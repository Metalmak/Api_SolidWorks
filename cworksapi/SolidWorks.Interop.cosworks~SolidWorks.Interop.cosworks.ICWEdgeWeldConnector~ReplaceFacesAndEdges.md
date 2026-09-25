<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector~ReplaceFacesAndEdges.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ReplaceFacesAndEdges Method (ICWEdgeWeldConnector) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWEdgeWeldConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector.html) : ReplaceFacesAndEdges Method (ICWEdgeWeldConnector) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NEdgeWeldStyle*
:   Type of edge weld connector as defined in [swsEdgeWeldConnectorTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsEdgeWeldConnectorTypes_e.html)

*DispFace1*
:   Face Set 1 array

*DispFace2*
:   Face Set 2 array

*Edges*
:   Array of edges between faces specified in DispFace1 and DispFace2

Replaces the current faces and edges in this edge weld connector with the specified faces and edges.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ReplaceFacesAndEdges( _    ByVal NEdgeWeldStyle As System.Integer, _    ByVal DispFace1 As System.Object, _    ByVal DispFace2 As System.Object, _    ByVal Edges As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWEdgeWeldConnector Dim NEdgeWeldStyle As System.Integer Dim DispFace1 As System.Object Dim DispFace2 As System.Object Dim Edges As System.Object Dim value As System.Integer   value = instance.ReplaceFacesAndEdges(NEdgeWeldStyle, DispFace1, DispFace2, Edges) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ReplaceFacesAndEdges(     System.int NEdgeWeldStyle,    System.object DispFace1,    System.object DispFace2,    System.object Edges ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ReplaceFacesAndEdges(  &   System.int NEdgeWeldStyle, &   System.Object^ DispFace1, &   System.Object^ DispFace2, &   System.Object^ Edges ) ``` | |

#### Parameters

*NEdgeWeldStyle*
:   Type of edge weld connector as defined in [swsEdgeWeldConnectorTypes\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsEdgeWeldConnectorTypes_e.html)

*DispFace1*
:   Face Set 1 array

*DispFace2*
:   Face Set 2 array

*Edges*
:   Array of edges between faces specified in DispFace1 and DispFace2

#### Return Value

Error code as defined in [swsWeldResultErrorCode\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsWeldResultErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWEdgeWeldConnector::ReplaceFacesAndEdges.

# ![](dotnetimages/collapse.gif)Example

See the [ICWEdgeWeldConnector](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWEdgeWeldConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector.html)

[ICWEdgeWeldConnector Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector_members.html)

[ICWEdgeWeldConnector::ReplaceFacesThenAutoGenerateTouchingEdges Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector~ReplaceFacesThenAutoGenerateTouchingEdges.html)

[ICWEdgeWeldConnector::AddEdges Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector~AddEdges.html)

[ICWEdgeWeldConnector::RemoveEdges Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector~RemoveEdges.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0