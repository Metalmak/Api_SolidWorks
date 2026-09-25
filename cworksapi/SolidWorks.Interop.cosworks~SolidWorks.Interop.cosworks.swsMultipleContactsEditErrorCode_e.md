<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMultipleContactsEditErrorCode_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsMultipleContactsEditErrorCode\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsMultipleContactsEditErrorCode\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Error codes for the simultaneous editing of component contacts and contact sets

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsMultipleContactsEditErrorCode_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsMultipleContactsEditErrorCode_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsMultipleContactsEditErrorCode_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsMultipleContactsEditErrorCode_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsMultipleContactsEditErrorCode\_BondedContactsWithBeamsCannotBeEditedWithOtherNonBeamContactTypes** | 12 = Bonded contact sets with beams cannot be edited together with other contact types |
| **swsMultipleContactsEditErrorCode\_GivenContactIsAlreadyAdded** | 8 = Contact has already been added |
| **swsMultipleContactsEditErrorCode\_GivenContactIsNotAddedYet** | 3 = Specified contact set is not yet added to the selection list |
| **swsMultipleContactsEditErrorCode\_GivenContactSetDidNotMeetMinCriteria** | 7 = Specified contact set/component contact does not meet the qualifying criteria for editing multiple contacts interactively |
| **swsMultipleContactsEditErrorCode\_InvalidPropertiesAreApplied** | 6 = Attempted to set one or more properties that are inconsistent with each other |
| **swsMultipleContactsEditErrorCode\_MultipleContactSetMgrIsNull** | 5 = Multiple contact sets cannot be simultaneously edited |
| **swsMultipleContactsEditErrorCode\_NoDefaultContactIsSelected** | 2 = Default contact must be set when the same type of contact is selected for editing |
| **swsMultipleContactsEditErrorCode\_NoPenetrationSelfContactSetsCannotBeEditedWithOtherContactTypes** | 10 = No Penetration self contact sets cannot be edited with other contact types |
| **swsMultipleContactsEditErrorCode\_NoSuchContactExists** | 4 = Specified name of contact set does not exist in the current study |
| **swsMultipleContactsEditErrorCode\_NoTypeSelectedForMixedContactTypesSelection** | 1 = Contact type must be set when different types of contacts are selected for editing |
| **swsMultipleContactsEditErrorCode\_OperationNotSupported** | 9 = Operation cannot be performed out of sequence |
| **swsMultipleContactsEditErrorCode\_Success** | 0 = Success |
| **swsMultipleContactsEditErrorCode\_VirtualWallContactSetsCannotBeEditedWithOtherContactTypes** | 11 = Virtual wall contact sets cannot be edited together with other contact types |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)