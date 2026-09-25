<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector~IsWeldOrientation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| IsWeldOrientation Method (ICWEdgeWeldConnector) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWEdgeWeldConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector.html) : IsWeldOrientation Method (ICWEdgeWeldConnector) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ErrorCode*
:   Error code as defined in [swsWeldResultErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsWeldResultErrorCode_e.html)

Gets whether to show the location of the weld with respect to the shell surface.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IsWeldOrientation( _    ByRef ErrorCode As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWEdgeWeldConnector Dim ErrorCode As System.Integer Dim value As System.Boolean   value = instance.IsWeldOrientation(ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IsWeldOrientation(     out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IsWeldOrientation(  &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*ErrorCode*
:   Error code as defined in [swsWeldResultErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsWeldResultErrorCode_e.html)

#### Return Value

True to show the location of the weld with respect to the shell surface, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWEdgeWeldConnector::IsWeldOrientation.

# ![](dotnetimages/collapse.gif)Example

See the [ICWEdgeWeldConnector](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only for single sided welds.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWEdgeWeldConnector Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector.html)

[ICWEdgeWeldConnector Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector_members.html)

[ICWEdgeWeldConnector::SetWeldOrientation Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector~SetWeldOrientation.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0