<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddSpringConnector.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddSpringConnector Method (ICWLoadsAndRestraintsManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html) : AddSpringConnector Method (ICWLoadsAndRestraintsManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NSpringSubType*
:   Spring connector type as defined in [swsSpringConnectorType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsSpringConnectorType_e.html)

*DispArrayComp1*
:   Array of planar faces, cylindrical faces, or vertices from a body depending on NSpringSubType

*DispArrayComp2*
:   Array of planar faces, cylindrical faces, or vertices, depending on NSpringSubType, from another body

*ErrorCode*
:   Error as defined in [swsSpringConnectorError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsSpringConnectorError_e.html)

Adds a spring connector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddSpringConnector( _    ByVal NSpringSubType As System.Integer, _    ByVal DispArrayComp1 As System.Object, _    ByVal DispArrayComp2 As System.Object, _    ByRef ErrorCode As System.Integer _ ) As CWSpringConnector ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadsAndRestraintsManager Dim NSpringSubType As System.Integer Dim DispArrayComp1 As System.Object Dim DispArrayComp2 As System.Object Dim ErrorCode As System.Integer Dim value As CWSpringConnector   value = instance.AddSpringConnector(NSpringSubType, DispArrayComp1, DispArrayComp2, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWSpringConnector AddSpringConnector(     System.int NSpringSubType,    System.object DispArrayComp1,    System.object DispArrayComp2,    ref System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWSpringConnector^ AddSpringConnector(  &   System.int NSpringSubType, &   System.Object^ DispArrayComp1, &   System.Object^ DispArrayComp2, &   System.int% ErrorCode ) ``` | |

#### Parameters

*NSpringSubType*
:   Spring connector type as defined in [swsSpringConnectorType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsSpringConnectorType_e.html)

*DispArrayComp1*
:   Array of planar faces, cylindrical faces, or vertices from a body depending on NSpringSubType

*DispArrayComp2*
:   Array of planar faces, cylindrical faces, or vertices, depending on NSpringSubType, from another body

*ErrorCode*
:   Error as defined in [swsSpringConnectorError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsSpringConnectorError_e.html)

#### Return Value

[Spring connector](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWSpringConnector.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadsAndRestraintsManager::AddSpringConnector.

# ![](dotnetimages/collapse.gif)Example

[Add Spring Connector (VBA)](Add_Spring_Connector_Example_VB.htm)

[Add Spring Connector (VB.NET)](Add_Spring_Connector_Example_VBNET.htm)

[Add Spring Connector (C#)](Add_Spring_Connector_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html)

[ICWLoadsAndRestraintsManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2009 SP0