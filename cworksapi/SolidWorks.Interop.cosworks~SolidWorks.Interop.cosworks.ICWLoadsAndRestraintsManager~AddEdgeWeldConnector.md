<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddEdgeWeldConnector.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddEdgeWeldConnector Method (ICWLoadsAndRestraintsManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html) : AddEdgeWeldConnector Method (ICWLoadsAndRestraintsManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FirstFace*
:   Array of Face Set1 faces

*SecondFace*
:   Array of Face Set2 faces

    | If NEdgeWeldStyle = swsEdgeWeldConnectorTypes\_e... | Then SecondFace array contains faces that are... |
    | --- | --- |
    | swsEdgeWeldConnectorGrooveDoubleSided  - or -  swsEdgeWeldConnectorGrooveSingleSided | Parallel to faces in FirstFace array |
    | swsEdgeWeldConnectorFilletDoubleSided  - or -  swsEdgeWeldConnectorFilletSingleSided | Perpendicular to faces in FirstFace array |

*Edges*
:   Array of touching edges between the faces specified in FirstFace and SecondFace arrays

*NEdgeWeldStyle*
:   Edge weld style as defined by [swsEdgeWeldConnectorTypes\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsEdgeWeldConnectorTypes_e.html)

*ErrorCode*
:   Error code as defined by [swsEdgeWeldCreationErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsEdgeWeldCreationErrorCode_e.html)

Creates the specified edge weld connector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddEdgeWeldConnector( _    ByVal FirstFace As System.Object, _    ByVal SecondFace As System.Object, _    ByVal Edges As System.Object, _    ByVal NEdgeWeldStyle As System.Integer, _    ByRef ErrorCode As System.Integer _ ) As CWEdgeWeldConnector ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadsAndRestraintsManager Dim FirstFace As System.Object Dim SecondFace As System.Object Dim Edges As System.Object Dim NEdgeWeldStyle As System.Integer Dim ErrorCode As System.Integer Dim value As CWEdgeWeldConnector   value = instance.AddEdgeWeldConnector(FirstFace, SecondFace, Edges, NEdgeWeldStyle, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWEdgeWeldConnector AddEdgeWeldConnector(     System.object FirstFace,    System.object SecondFace,    System.object Edges,    System.int NEdgeWeldStyle,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWEdgeWeldConnector^ AddEdgeWeldConnector(  &   System.Object^ FirstFace, &   System.Object^ SecondFace, &   System.Object^ Edges, &   System.int NEdgeWeldStyle, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*FirstFace*
:   Array of Face Set1 faces

*SecondFace*
:   Array of Face Set2 faces

    | If NEdgeWeldStyle = swsEdgeWeldConnectorTypes\_e... | Then SecondFace array contains faces that are... |
    | --- | --- |
    | swsEdgeWeldConnectorGrooveDoubleSided  - or -  swsEdgeWeldConnectorGrooveSingleSided | Parallel to faces in FirstFace array |
    | swsEdgeWeldConnectorFilletDoubleSided  - or -  swsEdgeWeldConnectorFilletSingleSided | Perpendicular to faces in FirstFace array |

*Edges*
:   Array of touching edges between the faces specified in FirstFace and SecondFace arrays

*NEdgeWeldStyle*
:   Edge weld style as defined by [swsEdgeWeldConnectorTypes\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsEdgeWeldConnectorTypes_e.html)

*ErrorCode*
:   Error code as defined by [swsEdgeWeldCreationErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsEdgeWeldCreationErrorCode_e.html)

#### Return Value

[ICWEdgeWeldConnector](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWEdgeWeldConnector.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadsAndRestraintsManager::AddEdgeWeldConnector.

# ![](dotnetimages/collapse.gif)Example

[Create and Edit Edge Weld Connector (VBA)](Create_and_Edit_Edge_Weld_Connector_Example_VB.htm)

[Create and Edit Edge Weld Connector (VB.NET)](Create_and_Edit_Edge_Weld_Connector_Example_VBNET.htm)

[Create and Edit Edge Weld Connector (C#)](Create_and_Edit_Edge_Weld_Connector_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html)

[ICWLoadsAndRestraintsManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager_members.html)

[ICWLoadsAndRestraintsManager::GetEdgeWeldConnector Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~GetEdgeWeldConnector.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0