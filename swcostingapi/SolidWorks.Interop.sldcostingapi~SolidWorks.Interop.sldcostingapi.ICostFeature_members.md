<!-- source: swcostingapi/SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostFeature_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Costing API Help | Send Feedback |
| ICostFeature Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldcostingapi Namespace](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi_namespace.html) : ICostFeature Interface |

The following tables list the members exposed by [ICostFeature](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostFeature.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [CombinedCost](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostFeature~CombinedCost.html) | Gets or sets the cost of this Costing feature or operation, including the combined cost of Costing child features and operations. |
| ![ Property](dotnetimages/Property.gif) | [CombinedTime](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostFeature~CombinedTime.html) | Gets or sets the time for this Costing feature or operation, including the combined times of Costing child features and operations. |
| ![ Property](dotnetimages/Property.gif) | [Description](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostFeature~Description.html) | Gets or sets the description of this Costing feature, including information about selected sub-operation options. |
| ![ Property](dotnetimages/Property.gif) | [IsOverridden](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostFeature~IsOverridden.html) | Gets whether a cost override was applied to this Costing feature. |
| ![ Property](dotnetimages/Property.gif) | [IsSetup](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostFeature~IsSetup.html) | Gets whether this Costing feature is a setup-related Costing feature. |
| ![ Property](dotnetimages/Property.gif) | [Name](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostFeature~Name.html) | Gets or sets the name of the Costing feature in the CostingManager. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [GetFirstSubFeature](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostFeature~GetFirstSubFeature.html) | Gets the first child feature that belongs to the Costing feature in the CostingManager. |
| ![ Method](dotnetimages/Method.gif) | [GetNextFeature](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostFeature~GetNextFeature.html) | Gets the next Costing feature in the CostingManager. |
| ![ Method](dotnetimages/Method.gif) | [GetNextSubFeature](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostFeature~GetNextSubFeature.html) | Gets the next Costing child feature from the owner of this Costing child feature in the CostingManager. |
| ![ Method](dotnetimages/Method.gif) | [GetType](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostFeature~GetType.html) | Gets the type of Costing feature in the CostingManager. |
| ![ Method](dotnetimages/Method.gif) | [RemoveOverrideCostTime](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostFeature~RemoveOverrideCostTime.html) | Removes the cost override and the time required for each operation to manufacture this Costing feature. |
| ![ Method](dotnetimages/Method.gif) | [SelectFaces](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostFeature~SelectFaces.html) | Selects the faces in the part affected by this Costing feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ICostFeature Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostFeature.html)

[SolidWorks.Interop.sldcostingapi Namespace](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi_namespace.html)

[ICostBody Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostBody.html)

[ICostPart Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostPart.html)