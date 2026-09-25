<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddCentrifugalForce.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddCentrifugalForce Method (ICWLoadsAndRestraintsManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html) : AddCentrifugalForce Method (ICWLoadsAndRestraintsManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DispEntity*
:   Reference geometry (axis, edge, or cylindrical face) to specify direction

*ErrorCode*
:   Error as defined in [swsCentrifugalForceError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsCentrifugalForceError_e.html)

Creates a centrifugal force.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddCentrifugalForce( _    ByVal DispEntity As System.Object, _    ByRef ErrorCode As System.Integer _ ) As CWCentriFugalForce ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadsAndRestraintsManager Dim DispEntity As System.Object Dim ErrorCode As System.Integer Dim value As CWCentriFugalForce   value = instance.AddCentrifugalForce(DispEntity, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWCentriFugalForce AddCentrifugalForce(     System.object DispEntity,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWCentriFugalForce^ AddCentrifugalForce(  &   System.Object^ DispEntity, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*DispEntity*
:   Reference geometry (axis, edge, or cylindrical face) to specify direction

*ErrorCode*
:   Error as defined in [swsCentrifugalForceError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsCentrifugalForceError_e.html)

#### Return Value

[Centrifugal force](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWCentriFugalForce.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadsAndRestraintsManager::AddCentrifugalForce.

# ![](dotnetimages/collapse.gif)Example

[Add Centrifugal Load (VBA)](Add_Centrifugal_Load_Example_VB.htm)

[Add Centrifugal Load (VB.NET)](Add_Centrifugal_Load_Example_VBNET.htm)

[Add Centrifugal Load (C#)](Add_Centrifugal_Load_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

The density material property must be specified to consider the effect of centrifugal loads.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html)

[ICWLoadsAndRestraintsManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0