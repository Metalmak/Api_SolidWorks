<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddPinConnector.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddPinConnector Method (ICWLoadsAndRestraintsManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html) : AddPinConnector Method (ICWLoadsAndRestraintsManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DispArrayComp1*
:   Array of one full cylindrical face or of multiple cylindrical faces of smaller angles belonging to the same body and coaxial with the same radius

*DispArrayComp2*
:   Array of one full cylindrical face or of multiple cylindrical faces of smaller angles belonging to the same body, but different than the body in DispArrayComp1, and coaxial with the same radius

*ErrorCode*
:   Error as defined in [swsPinConnectorError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsPinConnectorError_e.html)

Adds a pin connector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddPinConnector( _    ByVal DispArrayComp1 As System.Object, _    ByVal DispArrayComp2 As System.Object, _    ByRef ErrorCode As System.Integer _ ) As CWPinConnector ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadsAndRestraintsManager Dim DispArrayComp1 As System.Object Dim DispArrayComp2 As System.Object Dim ErrorCode As System.Integer Dim value As CWPinConnector   value = instance.AddPinConnector(DispArrayComp1, DispArrayComp2, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWPinConnector AddPinConnector(     System.object DispArrayComp1,    System.object DispArrayComp2,    ref System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWPinConnector^ AddPinConnector(  &   System.Object^ DispArrayComp1, &   System.Object^ DispArrayComp2, &   System.int% ErrorCode ) ``` | |

#### Parameters

*DispArrayComp1*
:   Array of one full cylindrical face or of multiple cylindrical faces of smaller angles belonging to the same body and coaxial with the same radius

*DispArrayComp2*
:   Array of one full cylindrical face or of multiple cylindrical faces of smaller angles belonging to the same body, but different than the body in DispArrayComp1, and coaxial with the same radius

*ErrorCode*
:   Error as defined in [swsPinConnectorError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsPinConnectorError_e.html)

#### Return Value

[Pin connector](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWPinConnector.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadsAndRestraintsManager::AddPinConnector.

# ![](dotnetimages/collapse.gif)Example

[Add Pin Connector (VBA)](Add_Pin_Connector_Example_VB.htm)

[Add Pin Connector (VB.NET)](Add_Pin_Connector_Example_VBNET.htm)

[Add Pin Connector (C#)](Add_Pin_Connector_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html)

[ICWLoadsAndRestraintsManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2009 SP0