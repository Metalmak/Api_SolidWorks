<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ICWContactManager Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : ICWContactManager Interface |

The following tables list the members exposed by [ICWContactManager](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [ContactComponentCount](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~ContactComponentCount.html) | Gets the number of component contacts in the active study. |
| ![ Property](dotnetimages/Property.gif) | [ContactSetCount](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~ContactSetCount.html) | Gets the number of contact sets in the active study. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [CopyContactsToStudy](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~CopyContactsToStudy.html) | Copies the specified contact sets to the specified study. |
| ![ Method](dotnetimages/Method.gif) | [CreateContactComponent](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~CreateContactComponent.html) | Creates the specified component contact. |
| ![ Method](dotnetimages/Method.gif) | [CreateContactSet](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~CreateContactSet.html) | Obsolete. Superseded by [ICWContactManager::CreateContactSet2](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWContactManager~CreateContactSet2.html). |
| ![ Method](dotnetimages/Method.gif) | [CreateContactSet2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~CreateContactSet2.html) | Creates a contact set. |
| ![ Method](dotnetimages/Method.gif) | [CreateContactSetsFromPairList](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~CreateContactSetsFromPairList.html) | Creates contact sets from the specified contact pairs. |
| ![ Method](dotnetimages/Method.gif) | [DeleteContactComponent](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~DeleteContactComponent.html) | Deletes the specified component contact. |
| ![ Method](dotnetimages/Method.gif) | [DeleteContactSet](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~DeleteContactSet.html) | Deletes the specified contact set. |
| ![ Method](dotnetimages/Method.gif) | [FindNonTouchingPairs](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~FindNonTouchingPairs.html) | Finds non-touching faces within the specified minimum and maximum distance in the specified bodies or components. |
| ![ Method](dotnetimages/Method.gif) | [FindTouchingEdgeFacePairs](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~FindTouchingEdgeFacePairs.html) | Finds touching shell edges and faces in the specified bodies or components. |
| ![ Method](dotnetimages/Method.gif) | [FindTouchingFacePairs](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~FindTouchingFacePairs.html) | Finds touching faces in the specified bodies or components. |
| ![ Method](dotnetimages/Method.gif) | [GetContactComponentAt](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~GetContactComponentAt.html) | Gets the component contact at the specified index. |
| ![ Method](dotnetimages/Method.gif) | [GetContactSetAt](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~GetContactSetAt.html) | Gets the contact set at the specified index. |
| ![ Method](dotnetimages/Method.gif) | [GetGlobalContact](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~GetGlobalContact.html) | Gets the contact type and options for global contact. |
| ![ Method](dotnetimages/Method.gif) | [SetGlobalContact](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~SetGlobalContact.html) | Sets the contact type and options for global contacts. |
| ![ Method](dotnetimages/Method.gif) | [SuppressUnsuppressComponentContact](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~SuppressUnsuppressComponentContact.html) | Obsolete. Superseded by [ICWContactManager::SuppressUnsuppressComponentContact2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~SuppressUnsuppressComponentContact2.html). |
| ![ Method](dotnetimages/Method.gif) | [SuppressUnsuppressComponentContact2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~SuppressUnsuppressComponentContact2.html) | Sets the suppression state of the specified component contact. |
| ![ Method](dotnetimages/Method.gif) | [SuppressUnsuppressContactPair](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~SuppressUnsuppressContactPair.html) | Obsolete. Superseded by [ICWContactManager::SuppressUnsuppressContactPair2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~SuppressUnsuppressContactPair2.html). |
| ![ Method](dotnetimages/Method.gif) | [SuppressUnsuppressContactPair2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager~SuppressUnsuppressContactPair2.html) | Sets the suppression state of the specified contact set. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWContactManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager.html)

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)

[ICWContactComponent Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent.html)

[ICWContactSet Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactSet.html)

[ICWMultipleComponentContactsEditManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager.html)

[ICWMultipleContactSetsEditManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleContactSetsEditManager.html)