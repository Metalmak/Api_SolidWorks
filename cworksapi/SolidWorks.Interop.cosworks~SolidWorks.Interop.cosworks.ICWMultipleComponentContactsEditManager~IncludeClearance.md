<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager~IncludeClearance.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| IncludeClearance Method (ICWMultipleComponentContactsEditManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWMultipleComponentContactsEditManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager.html) : IncludeClearance Method (ICWMultipleComponentContactsEditManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BNonTouching*
:   1 to include clearance for non-touching faces, 0 to not

Obsolete. Superseded by [ICWMultipleComponentContactsEditManager::IncludeClearance2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager~IncludeClearance2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IncludeClearance( _    ByVal BNonTouching As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWMultipleComponentContactsEditManager Dim BNonTouching As System.Integer Dim value As System.Integer   value = instance.IncludeClearance(BNonTouching) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IncludeClearance(     System.int BNonTouching ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IncludeClearance(  &   System.int BNonTouching ) ``` | |

#### Parameters

*BNonTouching*
:   1 to include clearance for non-touching faces, 0 to not

#### Return Value

Error code as defined in [swsMultipleContactsEditErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMultipleContactsEditErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWMultipleComponentContactsEditManager::IncludeClearance.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWMultipleComponentContactsEditManager::SetContactType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager~SetContactType.html)'s NType is set to [swsContactType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsContactType_e.html).swsContactTypeBonded.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWMultipleComponentContactsEditManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager.html)

[ICWMultipleComponentContactsEditManager Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager_members.html)

[ICWMultipleComponentContactsEditManager::SetClearanceUnit Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager~SetClearanceUnit.html)

[ICWMultipleComponentContactsEditManager::SetClearanceValue Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager~SetClearanceValue.html)

**ICWMultipleComponentContactsEditManager::GetClearanceUnit Method ()**

**ICWMultipleComponentContactsEditManager::GetClearanceValue Method ()**

**ICWMultipleComponentContactsEditManager::GetIncludeClearance Method ()**

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0