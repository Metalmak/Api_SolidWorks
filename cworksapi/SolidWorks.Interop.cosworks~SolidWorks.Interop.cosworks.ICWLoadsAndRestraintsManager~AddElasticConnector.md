<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddElasticConnector.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddElasticConnector Method (ICWLoadsAndRestraintsManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html) : AddElasticConnector Method (ICWLoadsAndRestraintsManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DispArray*
:   Array of faces for the elastic support fixture

*ErrorCode*
:   Error as defined in [swsElasticConnectorError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsElasticConnectorError_e.html)

Adds an elastic support fixture.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddElasticConnector( _    ByVal DispArray As System.Object, _    ByRef ErrorCode As System.Integer _ ) As CWElasticConnector ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadsAndRestraintsManager Dim DispArray As System.Object Dim ErrorCode As System.Integer Dim value As CWElasticConnector   value = instance.AddElasticConnector(DispArray, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWElasticConnector AddElasticConnector(     System.object DispArray,    ref System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWElasticConnector^ AddElasticConnector(  &   System.Object^ DispArray, &   System.int% ErrorCode ) ``` | |

#### Parameters

*DispArray*
:   Array of faces for the elastic support fixture

*ErrorCode*
:   Error as defined in [swsElasticConnectorError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsElasticConnectorError_e.html)

#### Return Value

[Elastic support fixture](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWElasticConnector.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadsAndRestraintsManager::AddElasticConnector.

# ![](dotnetimages/collapse.gif)Example

[Add Elastic Support Fixture (VBA)](Add_Elastic_Support_Connector_Example_VB.htm)

[Add Elastic Support Fixture (VB.NET)](Add_Elastic_Support_Connector_Example_VBNET.htm)

[Add Elastic Support Fixture (C#)](Add_Elastic_Support_Connector_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html)

[ICWLoadsAndRestraintsManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2009 SP0