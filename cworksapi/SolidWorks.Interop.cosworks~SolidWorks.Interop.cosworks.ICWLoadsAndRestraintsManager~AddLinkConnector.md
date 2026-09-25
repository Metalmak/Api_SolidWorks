<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddLinkConnector.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddLinkConnector Method (ICWLoadsAndRestraintsManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html) : AddLinkConnector Method (ICWLoadsAndRestraintsManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*VertexPointforFirstLocation*
:   Vertex for first location

*VertexPointforSecondLocation*
:   Vertex for second location

*ErrorCode*
:   Error as defined in [swsLinkConnectorError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLinkConnectorError_e.html)

Adds a link connector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddLinkConnector( _    ByVal VertexPointforFirstLocation As System.Object, _    ByVal VertexPointforSecondLocation As System.Object, _    ByRef ErrorCode As System.Integer _ ) As CWLinkConnector ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadsAndRestraintsManager Dim VertexPointforFirstLocation As System.Object Dim VertexPointforSecondLocation As System.Object Dim ErrorCode As System.Integer Dim value As CWLinkConnector   value = instance.AddLinkConnector(VertexPointforFirstLocation, VertexPointforSecondLocation, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWLinkConnector AddLinkConnector(     System.object VertexPointforFirstLocation,    System.object VertexPointforSecondLocation,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWLinkConnector^ AddLinkConnector(  &   System.Object^ VertexPointforFirstLocation, &   System.Object^ VertexPointforSecondLocation, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*VertexPointforFirstLocation*
:   Vertex for first location

*VertexPointforSecondLocation*
:   Vertex for second location

*ErrorCode*
:   Error as defined in [swsLinkConnectorError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLinkConnectorError_e.html)

#### Return Value

[Link connector](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWLinkConnector.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadsAndRestraintsManager::AddLinkConnector.

# ![](dotnetimages/collapse.gif)Example

See the [ICWLinkConnector](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLinkConnector.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html)

[ICWLoadsAndRestraintsManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2009 SP0