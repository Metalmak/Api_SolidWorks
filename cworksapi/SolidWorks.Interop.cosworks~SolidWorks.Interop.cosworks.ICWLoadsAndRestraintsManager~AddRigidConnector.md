<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddRigidConnector.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddRigidConnector Method (ICWLoadsAndRestraintsManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html) : AddRigidConnector Method (ICWLoadsAndRestraintsManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PersistIDFaceArray*
:   Array of objects of the faces from a solid body

*PersistIDTargetArray*
:   Array of objects of the faces from the target solid body

*ErrorCode*
:   Error as defined in [swsRigidConnectorError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsRigidConnectorError_e.html)

Adds a rigid connector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddRigidConnector( _    ByVal PersistIDFaceArray As System.Object, _    ByVal PersistIDTargetArray As System.Object, _    ByRef ErrorCode As System.Integer _ ) As CWRigidConnector ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadsAndRestraintsManager Dim PersistIDFaceArray As System.Object Dim PersistIDTargetArray As System.Object Dim ErrorCode As System.Integer Dim value As CWRigidConnector   value = instance.AddRigidConnector(PersistIDFaceArray, PersistIDTargetArray, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWRigidConnector AddRigidConnector(     System.object PersistIDFaceArray,    System.object PersistIDTargetArray,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWRigidConnector^ AddRigidConnector(  &   System.Object^ PersistIDFaceArray, &   System.Object^ PersistIDTargetArray, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*PersistIDFaceArray*
:   Array of objects of the faces from a solid body

*PersistIDTargetArray*
:   Array of objects of the faces from the target solid body

*ErrorCode*
:   Error as defined in [swsRigidConnectorError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsRigidConnectorError_e.html)

#### Return Value

[Rigid connector](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWRigidConnector.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadsAndRestraintsManager::AddRigidConnector.

# ![](dotnetimages/collapse.gif)Example

[Add Rigid Connector (VBA)](Add_Rigid_Connector_Example_VB.htm)

[Add Rigid Connector (VB.NET)](Add_Rigid_Connector_Example_VBNET.htm)

[Add Rigid Connector (C#)](Add_Rigid_Connector_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html)

[ICWLoadsAndRestraintsManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2009 SP0