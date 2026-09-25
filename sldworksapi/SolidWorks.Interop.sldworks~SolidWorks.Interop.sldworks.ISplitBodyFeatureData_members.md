<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISplitBodyFeatureData Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ISplitBodyFeatureData Interface |

The following tables list the members exposed by [ISplitBodyFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [Consume](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData~Consume.html) | Gets or sets whether the bodies in this Split feature are consumed. |
| ![ Property](dotnetimages/Property.gif) | [OverrideDefaultTemplateSettings](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData~OverrideDefaultTemplateSettings.html) | Gets or sets whether to use an alternate template to apply to all new part or assembly files created during the split operation. |
| ![ Property](dotnetimages/Property.gif) | [TemplatePath](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData~TemplatePath.html) | Gets or sets the template to use to make this Split feature. |
| ![ Property](dotnetimages/Property.gif) | [TrimTools](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData~TrimTools.html) | Gets the trimming surfaces used as trim tools in this Split feature.  **NOTE:** **This property is a get-only property.** **Set is not implemented**. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData~AccessSelections.html) | Gains access to a Split feature. |
| ![ Method](dotnetimages/Method.gif) | [GetSplitBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData~GetSplitBodies.html) | Gets the split bodies in this Split feature. |
| ![ Method](dotnetimages/Method.gif) | [GetSplitBodiesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData~GetSplitBodiesCount.html) | Gets the number of split bodies in this Split feature. |
| ![ Method](dotnetimages/Method.gif) | [GetTrimToolsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData~GetTrimToolsCount.html) | Gets the number of trimming surfaces used as trim tools in this Split feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetSplitBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData~IGetSplitBodies.html) | Gets the split bodies for this Split feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetTrimTools](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData~IGetTrimTools.html) | Gets the trimming surfaces used as trim tools in this Split feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetSplitBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData~ISetSplitBodies.html) | Obsolete. Superseded by [ISplitBodyFeatureData::SetSplitBodies2.](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISplitBodyFeatureData~SetSplitBodies2.html) |
| ![ Method](dotnetimages/Method.gif) | [ISetTrimTools](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData~ISetTrimTools.html) | Gets the trimming surfaces used as trim tools in this Split feature. |
| ![ Method](dotnetimages/Method.gif) | [ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData~ReleaseSelectionAccess.html) | Releases access to the selections that define this Split feature. |
| ![ Method](dotnetimages/Method.gif) | [SetSplitBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData~SetSplitBodies.html) | Obsolete. Superseded by [ISplitBodyFeatureData::SetSplitBodies2.](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISplitBodyFeatureData~SetSplitBodies2.html) |
| ![ Method](dotnetimages/Method.gif) | [SetSplitBodies2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData~SetSplitBodies2.html) | Edits the current split bodies in this Split feature. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ISplitBodyFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISplitBodyFeatureData.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IFeatureManager::PreSplitBody Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~PreSplitBody.html)