<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~GetEdgeWeldConnector.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetEdgeWeldConnector Method (ICWLoadsAndRestraintsManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html) : GetEdgeWeldConnector Method (ICWLoadsAndRestraintsManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NIndex*
:   Index of the edge weld connector to get (see **Remarks**)

*ErrorCode*
:   Error code as defined by [swsEdgeWeldCreationErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsEdgeWeldCreationErrorCode_e.html)

Gets the edge weld connector at the specified index.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetEdgeWeldConnector( _    ByVal NIndex As System.Integer, _    ByRef ErrorCode As System.Integer _ ) As CWEdgeWeldConnector ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadsAndRestraintsManager Dim NIndex As System.Integer Dim ErrorCode As System.Integer Dim value As CWEdgeWeldConnector   value = instance.GetEdgeWeldConnector(NIndex, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWEdgeWeldConnector GetEdgeWeldConnector(     System.int NIndex,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWEdgeWeldConnector^ GetEdgeWeldConnector(  &   System.int NIndex, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*NIndex*
:   Index of the edge weld connector to get (see **Remarks**)

*ErrorCode*
:   Error code as defined by [swsEdgeWeldCreationErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsEdgeWeldCreationErrorCode_e.html)

#### Return Value

[ICWEdgeWeldConnector](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadsAndRestraintsManager::GetEdgeWeldConnector.

# ![](dotnetimages/collapse.gif)Example

[Create and Edit Edge Weld Connector (VBA)](Create_and_Edit_Edge_Weld_Connector_Example_VB.htm)

[Create and Edit Edge Weld Connector (VB.NET)](Create_and_Edit_Edge_Weld_Connector_Example_VBNET.htm)

[Create and Edit Edge Weld Connector (C#)](Create_and_Edit_Edge_Weld_Connector_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call [ICWLoadsAndRestraintsManager::Count](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~Count.html) to determine NIndex. The vertical position of a load or restraint in the Simulation Study tree does not correspond to NIndex. You must use [ICWLoadsAndRestraintsManager::GetLoadsAndRestraints](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~GetLoadsAndRestraints.html) to determine the mapping between NIndex and the study's loads and restraints.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html)

[ICWLoadsAndRestraintsManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager_members.html)

[ICWLoadsAndRestraintsManager::AddEdgeWeldConnector Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddEdgeWeldConnector.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0