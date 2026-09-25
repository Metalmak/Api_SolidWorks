<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddRemoteLoad.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddRemoteLoad Method (ICWLoadsAndRestraintsManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html) : AddRemoteLoad Method (ICWLoadsAndRestraintsManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NLoadType*
:   Type of restraint or load as defined in [swsRemoteLoadType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsRemoteLoadType_e.html)

*DispArray*
:   | If NLoadType is ... | Then DispArray is an array of ... |
    | --- | --- |
    | [swsRemoteLoadType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsRemoteLoadType_e.html).swsRemoteLoadType\_RigidLoadOrMass  - or -  [swsRemoteLoadType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsRemoteLoadType_e.html).swsRemoteLoadType\_RigidDisplacement | Faces, edges, or vertices |
    | [swsRemoteLoadType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsRemoteLoadType_e.html).swsRemoteLoadType\_DirectLoad  - or -  [swsRemoteLoadType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsRemoteLoadType_e.html).swsRemoteLoadType\_DirectDisplacement | Faces |

*NLocationUnits*
:   Units as defined in [swsLinearUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLinearUnit_e.html)

*DXValue*
:   X-coordinate of the point of application of the remote load

*DYValue*
:   Y-coordinate of the point of application of the remote load

*DZValue*
:   Z-coordinate of the point of application of the remote load

*ErrorCode*
:   Error code as defined in [swsLoadsAndRestraintsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLoadsAndRestraintsError_e.html)

Creates a remote load of the specified type at the specified location.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddRemoteLoad( _    ByVal NLoadType As System.Integer, _    ByVal DispArray As System.Object, _    ByVal NLocationUnits As System.Integer, _    ByVal DXValue As System.Double, _    ByVal DYValue As System.Double, _    ByVal DZValue As System.Double, _    ByRef ErrorCode As System.Integer _ ) As CWRemoteLoad ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadsAndRestraintsManager Dim NLoadType As System.Integer Dim DispArray As System.Object Dim NLocationUnits As System.Integer Dim DXValue As System.Double Dim DYValue As System.Double Dim DZValue As System.Double Dim ErrorCode As System.Integer Dim value As CWRemoteLoad   value = instance.AddRemoteLoad(NLoadType, DispArray, NLocationUnits, DXValue, DYValue, DZValue, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWRemoteLoad AddRemoteLoad(     System.int NLoadType,    System.object DispArray,    System.int NLocationUnits,    System.double DXValue,    System.double DYValue,    System.double DZValue,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWRemoteLoad^ AddRemoteLoad(  &   System.int NLoadType, &   System.Object^ DispArray, &   System.int NLocationUnits, &   System.double DXValue, &   System.double DYValue, &   System.double DZValue, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*NLoadType*
:   Type of restraint or load as defined in [swsRemoteLoadType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsRemoteLoadType_e.html)

*DispArray*
:   | If NLoadType is ... | Then DispArray is an array of ... |
    | --- | --- |
    | [swsRemoteLoadType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsRemoteLoadType_e.html).swsRemoteLoadType\_RigidLoadOrMass  - or -  [swsRemoteLoadType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsRemoteLoadType_e.html).swsRemoteLoadType\_RigidDisplacement | Faces, edges, or vertices |
    | [swsRemoteLoadType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsRemoteLoadType_e.html).swsRemoteLoadType\_DirectLoad  - or -  [swsRemoteLoadType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsRemoteLoadType_e.html).swsRemoteLoadType\_DirectDisplacement | Faces |

*NLocationUnits*
:   Units as defined in [swsLinearUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLinearUnit_e.html)

*DXValue*
:   X-coordinate of the point of application of the remote load

*DYValue*
:   Y-coordinate of the point of application of the remote load

*DZValue*
:   Z-coordinate of the point of application of the remote load

*ErrorCode*
:   Error code as defined in [swsLoadsAndRestraintsError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLoadsAndRestraintsError_e.html)

#### Return Value

[ICWRemoteLoad](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWRemoteLoad.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadsAndRestraintsManager::AddRemoteLoad.

# ![](dotnetimages/collapse.gif)Example

[Add Remote Load (VBA)](Add_Remote_Load_Example_VB.htm)

[Add Remote Load (VB.NET)](Add_Remote_Load_Example_VBNET.htm)

[Add Remote Load (C#)](Add_Remote_Load_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html)

[ICWLoadsAndRestraintsManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0