<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ICWContactComponent Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : ICWContactComponent Interface |

The following tables list the members exposed by [ICWContactComponent](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [BondingFormulation](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~BondingFormulation.html) | Sets the bonding formulation for this contact. |
| ![ Property](dotnetimages/Property.gif) | [ClearanceUnit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~ClearanceUnit.html) | Gets or sets the units of clearance between non-touching faces. |
| ![ Property](dotnetimages/Property.gif) | [ClearanceValue](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~ClearanceValue.html) | Gets or sets the maximum clearance (gap) between non-touching faces or shell edges. |
| ![ Property](dotnetimages/Property.gif) | [ContactComponentType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~ContactComponentType.html) | Gets or sets the type of contact. |
| ![ Property](dotnetimages/Property.gif) | [ContactName](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~ContactName.html) | Gets the name of the contact. |
| ![ Property](dotnetimages/Property.gif) | [FrictionValue](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~FrictionValue.html) | Gets or sets the friction coefficient for this contact. |
| ![ Property](dotnetimages/Property.gif) | [GlobalContact](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~GlobalContact.html) | Obsolete. Superseded by [ICWContactComponent::GlobalContact2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~GlobalContact2.html). |
| ![ Property](dotnetimages/Property.gif) | [GlobalContact2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~GlobalContact2.html) | Sets whether to apply a global contact condition. |
| ![ Property](dotnetimages/Property.gif) | [IncludeClearance](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~IncludeClearance.html) | Obsolete. Superseded by [ICWContactComponent::IncludeClearance2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~IncludeClearance2.html). |
| ![ Property](dotnetimages/Property.gif) | [IncludeClearance2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~IncludeClearance2.html) | Sets whether to specify clearance for non-touching faces in this contact. |
| ![ Property](dotnetimages/Property.gif) | [IncludeFriction](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~IncludeFriction.html) | Obsolete. Superseded by [ICWContactComponent::IncludeFriction2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~IncludeFriction2.html). |
| ![ Property](dotnetimages/Property.gif) | [IncludeFriction2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~IncludeFriction2.html) | Sets whether to specify a friction coefficient for this contact. |
| ![ Property](dotnetimages/Property.gif) | [IncludeShellEdgeSolidOrShellFace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~IncludeShellEdgeSolidOrShellFace.html) | Obsolete. Superseded by [ICWContactComponent::IncludeShellEdgeSolidOrShellFace2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~IncludeShellEdgeSolidOrShellFace2.html). |
| ![ Property](dotnetimages/Property.gif) | [IncludeShellEdgeSolidOrShellFace2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~IncludeShellEdgeSolidOrShellFace2.html) | Sets whether to create contact sets. |
| ![ Property](dotnetimages/Property.gif) | [Option](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~Option.html) | Gets or sets the mesh compatibility for this contact. |
| ![ Property](dotnetimages/Property.gif) | [State](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~State.html) | Gets the suppression state of this contact. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [ContactComponentBeginEdit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~ContactComponentBeginEdit.html) | Start editing of this contact. |
| ![ Method](dotnetimages/Method.gif) | [ContactComponentEndEdit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~ContactComponentEndEdit.html) | Ends editing of this contact. |
| ![ Method](dotnetimages/Method.gif) | [InsertEntity](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~InsertEntity.html) | Inserts a component into this contact. |
| ![ Method](dotnetimages/Method.gif) | [RemoveEntity](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~RemoveEntity.html) | Removes a component from this contact. |
| ![ Method](dotnetimages/Method.gif) | [ReplaceEntity](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~ReplaceEntity.html) | Replaces the entity of this contact. |
| ![ Method](dotnetimages/Method.gif) | [SuppressUnSuppress](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent~SuppressUnSuppress.html) | Suppresses or unsuppresses this contact depending on its [state](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWContactComponent~State.html). |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWContactComponent Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactComponent.html)

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)

[ICWContactManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactManager.html)

[ICWContactSet Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactSet.html)

[ICWMultipleComponentContactsEditManager Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMultipleComponentContactsEditManager.html)