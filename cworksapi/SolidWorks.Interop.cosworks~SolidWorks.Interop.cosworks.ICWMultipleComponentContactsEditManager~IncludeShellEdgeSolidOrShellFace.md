<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager~IncludeShellEdgeSolidOrShellFace.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| IncludeShellEdgeSolidOrShellFace Method (ICWMultipleComponentContactsEditManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMultipleComponentContactsEditManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager.html) : IncludeShellEdgeSolidOrShellFace Method (ICWMultipleComponentContactsEditManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BNonTouchingShell*
:   1 to create edge-to-edge bonded contact sets, 0 to not

Obsolete. Superseded by [ICWMultipleComponentContactsEditManager::IncludeShellEdgeSolidOrShellFace2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager~IncludeShellEdgeSolidOrShellFace2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IncludeShellEdgeSolidOrShellFace( _    ByVal BNonTouchingShell As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMultipleComponentContactsEditManager Dim BNonTouchingShell As System.Integer Dim value As System.Integer   value = instance.IncludeShellEdgeSolidOrShellFace(BNonTouchingShell) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IncludeShellEdgeSolidOrShellFace(     System.int BNonTouchingShell ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IncludeShellEdgeSolidOrShellFace(  &   System.int BNonTouchingShell ) ``` | |

#### Parameters

*BNonTouchingShell*
:   1 to create edge-to-edge bonded contact sets, 0 to not

#### Return Value

Error code as defined in [swsMultipleContactsEditErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMultipleContactsEditErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMultipleComponentContactsEditManager::IncludeShellEdgeSolidOrShellFace.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if:

* [ICWMultipleComponentContactsEditManager::IncludeClearance](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager~IncludeClearance.html)'s BNonTouching is set to 1,

    - and -

* [ICWMultipleComponentContactsEditManager::SetContactType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager~SetContactType.html)'s NType is set to [swsContactType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsContactType_e.html).swsContactTypeBonded.

If BNonTouchingShell is set to true, then this method creates edge-to-edge bonded contact sets for pairs of:

* shell edges-to-shell edges,* shell edges-to-shell faces, and* shell edges-to-solid faces

that are within clearance as specified by [ICWMultipleComponentContactsEditManager::SetClearanceValue](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager~SetClearanceValue.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMultipleComponentContactsEditManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager.html)

[ICWMultipleComponentContactsEditManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager_members.html)

**ICWMultipleComponentContactsEditManager::GetIncludeShellEdgeSolidOrShellFace Method ()**

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0