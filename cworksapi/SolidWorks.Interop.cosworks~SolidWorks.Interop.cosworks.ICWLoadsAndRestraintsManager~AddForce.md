<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager~AddForce.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AddForce Method (ICWLoadsAndRestraintsManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html) : AddForce Method (ICWLoadsAndRestraintsManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NForceType*
:   Type of force as defined in [swsForceType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsForceType_e.html)

*DispArray*
:   Array of entities (faces, edges, vertices, or points) to which to apply force

*RefGeom*
:   Reference geometry entity to specify direction (see **Remarks**)

*ErrorCode*
:   Error as defined in [swsForceError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsForceError_e.html)

Obsolete. Superseded by [ICWLoadsAndRestraintsManager::AddForce2](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWLoadsAndRestraintsManager~AddForce2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddForce( _    ByVal NForceType As System.Integer, _    ByVal DispArray As System.Object, _    ByVal RefGeom As System.Object, _    ByRef ErrorCode As System.Integer _ ) As CWForce ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWLoadsAndRestraintsManager Dim NForceType As System.Integer Dim DispArray As System.Object Dim RefGeom As System.Object Dim ErrorCode As System.Integer Dim value As CWForce   value = instance.AddForce(NForceType, DispArray, RefGeom, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWForce AddForce(     System.int NForceType,    System.object DispArray,    System.object RefGeom,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWForce^ AddForce(  &   System.int NForceType, &   System.Object^ DispArray, &   System.Object^ RefGeom, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*NForceType*
:   Type of force as defined in [swsForceType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsForceType_e.html)

*DispArray*
:   Array of entities (faces, edges, vertices, or points) to which to apply force

*RefGeom*
:   Reference geometry entity to specify direction (see **Remarks**)

*ErrorCode*
:   Error as defined in [swsForceError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsForceError_e.html)

#### Return Value

[Force](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWForce.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWLoadsAndRestraintsManager::AddForce.

# ![](dotnetimages/collapse.gif)Remarks

Pass null in RefGeom if reference geometry is not used.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWLoadsAndRestraintsManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager.html)

[ICWLoadsAndRestraintsManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWLoadsAndRestraintsManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008, SP1.0