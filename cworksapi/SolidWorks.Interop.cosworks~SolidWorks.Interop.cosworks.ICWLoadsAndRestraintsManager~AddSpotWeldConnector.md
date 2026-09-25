<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddSpotWeldConnector.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddSpotWeldConnector Method (ICWLoadsAndRestraintsManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html) : AddSpotWeldConnector Method (ICWLoadsAndRestraintsManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FirstFace*
:   Face of a shell or solid body

*SecondFace*
:   Face of a shell or solid body that belongs to a different body than FirstFace

*DispArrayWeldLocations*
:   Array of vertices or an array of reference points to project on the faces to determine the locations of the spot welds

*ErrorCode*
:   Error as defined in [swsSpotWeldConnectorError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsSpotWeldConnectorError_e.html)

Adds a spot weld connector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddSpotWeldConnector( _    ByVal FirstFace As System.Object, _    ByVal SecondFace As System.Object, _    ByVal DispArrayWeldLocations As System.Object, _    ByRef ErrorCode As System.Integer _ ) As CWSpotWeldConnector ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadsAndRestraintsManager Dim FirstFace As System.Object Dim SecondFace As System.Object Dim DispArrayWeldLocations As System.Object Dim ErrorCode As System.Integer Dim value As CWSpotWeldConnector   value = instance.AddSpotWeldConnector(FirstFace, SecondFace, DispArrayWeldLocations, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWSpotWeldConnector AddSpotWeldConnector(     System.object FirstFace,    System.object SecondFace,    System.object DispArrayWeldLocations,    ref System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWSpotWeldConnector^ AddSpotWeldConnector(  &   System.Object^ FirstFace, &   System.Object^ SecondFace, &   System.Object^ DispArrayWeldLocations, &   System.int% ErrorCode ) ``` | |

#### Parameters

*FirstFace*
:   Face of a shell or solid body

*SecondFace*
:   Face of a shell or solid body that belongs to a different body than FirstFace

*DispArrayWeldLocations*
:   Array of vertices or an array of reference points to project on the faces to determine the locations of the spot welds

*ErrorCode*
:   Error as defined in [swsSpotWeldConnectorError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsSpotWeldConnectorError_e.html)

#### Return Value

[Spot weld connector](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWSpotWeldConnector.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadsAndRestraintsManager::AddSpotWeldConnector.

# ![](dotnetimages/collapse.gif)Example

[Add Spot Weld Connector (VBA)](Add_Spot_Weld_Connector_Example_VB.htm)

[Add Spot Weld Connector (VB.NET)](Add_Spot_Weld_Connector_Example_VBNET.htm)

[Add Spot Weld Connector (C#)](Add_Spot_Weld_Connector_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html)

[ICWLoadsAndRestraintsManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2009 SP0