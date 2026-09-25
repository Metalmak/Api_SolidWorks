<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IDrSection Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IDrSection Interface |

The following tables list the members exposed by [IDrSection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [CutSurfaceBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~CutSurfaceBodies.html) | Gets or sets whether to hide cut surface bodies in this section view. |
| ![ Property](dotnetimages/Property.gif) | [CuttingLineShoulders](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~CuttingLineShoulders.html) | Gets or sets whether to hide cutting line shoulders in this section view. |
| ![ Property](dotnetimages/Property.gif) | [DisplaySurfaceBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~DisplaySurfaceBodies.html) | Gets or sets whether to display surface bodies in this section view. |
| ![ Property](dotnetimages/Property.gif) | [ExcludeFasteners](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~ExcludeFasteners.html) | Gets or sets whether to exclude fasteners in the section view. |
| ![ Property](dotnetimages/Property.gif) | [ExcludeSliceSectionBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~ExcludeSliceSectionBodies.html) | Gets or sets whether to exclude slice section bodies in this section view. |
| ![ Property](dotnetimages/Property.gif) | [Layer](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~Layer.html) | Gets or sets the name of the layer on which the section line lies. |
| ![ Property](dotnetimages/Property.gif) | [RandomizeScale](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~RandomizeScale.html) | Gets or sets whether to randomize the scale when auto hatching this section view. |
| ![ Property](dotnetimages/Property.gif) | [ScaleHatchPattern](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~ScaleHatchPattern.html) | Gets or sets whether to scale the hatch pattern to the section view. |
| ![ Property](dotnetimages/Property.gif) | [SectionDepth](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~SectionDepth.html) | Gets or sets the distance from the section line of the section view. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [EnumExcludedComponents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~EnumExcludedComponents.html) | Obsolete. Superseded by [IDrSection::EnumExcludedComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrSection~EnumExcludedComponents2.html). |
| ![ Method](dotnetimages/Method.gif) | [EnumExcludedComponents2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~EnumExcludedComponents2.html) | Gets all of the assembly components that are excluded from this section view. |
| ![ Method](dotnetimages/Method.gif) | [GetArrowInfo](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~GetArrowInfo.html) | Gets the position of the arrows for the section line. |
| ![ Method](dotnetimages/Method.gif) | [GetAutoHatch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~GetAutoHatch.html) | Gets whether auto hatching is enabled for the section view resulting from this section cut. |
| ![ Method](dotnetimages/Method.gif) | [GetDisplayOnlySpeedPakBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~GetDisplayOnlySpeedPakBodies.html) | Gets whether to display in this section view only the bodies included in the SpeedPak configuration. |
| ![ Method](dotnetimages/Method.gif) | [GetDisplayOnlySurfaceCut](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~GetDisplayOnlySurfaceCut.html) | Gets whether to display only the surface cut by the section line. |
| ![ Method](dotnetimages/Method.gif) | [GetDontCutAllInstances](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~GetDontCutAllInstances.html) | Gets whether all instances of the specified component are uncut in this section view or only in the specified component. |
| ![ Method](dotnetimages/Method.gif) | [GetExcludedComponents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~GetExcludedComponents.html) | Gets all of the assembly components that are excluded from this section view. |
| ![ Method](dotnetimages/Method.gif) | [GetLabel](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~GetLabel.html) | Gets the label for this section view. |
| ![ Method](dotnetimages/Method.gif) | [GetLineInfo](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~GetLineInfo.html) | Gets the vertices of the section line. |
| ![ Method](dotnetimages/Method.gif) | [GetName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~GetName.html) | Gets the name of the section line. |
| ![ Method](dotnetimages/Method.gif) | [GetPartialSection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~GetPartialSection.html) | Gets whether this is a partial section cut. |
| ![ Method](dotnetimages/Method.gif) | [GetReversedCutDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~GetReversedCutDirection.html) | Gets whether the section cut direction is reversed from the default direction. |
| ![ Method](dotnetimages/Method.gif) | [GetScaleWithModelChanges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~GetScaleWithModelChanges.html) | Gets whether the section line scales with changes to the model. |
| ![ Method](dotnetimages/Method.gif) | [GetSectionView](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~GetSectionView.html) | Gets the section view of this section cut. |
| ![ Method](dotnetimages/Method.gif) | [GetTextFormat](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~GetTextFormat.html) | Gets the text format for the text for this section line. |
| ![ Method](dotnetimages/Method.gif) | [GetTextInfo](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~GetTextInfo.html) | Gets the location of the section line text. |
| ![ Method](dotnetimages/Method.gif) | [GetUseDocTextFormat](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~GetUseDocTextFormat.html) | Gets whether SOLIDWORKS is currently using the document default setting for text format. |
| ![ Method](dotnetimages/Method.gif) | [GetView](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~GetView.html) | Gets the drawing view where the section line appears. |
| ![ Method](dotnetimages/Method.gif) | [IGetArrowInfo](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~IGetArrowInfo.html) | Gets the position of the arrows for this section line. |
| ![ Method](dotnetimages/Method.gif) | [IGetLineInfo](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~IGetLineInfo.html) | Gets the vertices of the section line. |
| ![ Method](dotnetimages/Method.gif) | [IGetLineSegmentCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~IGetLineSegmentCount.html) | Gets the number of line segments making up this section line. |
| ![ Method](dotnetimages/Method.gif) | [IGetSectionView](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~IGetSectionView.html) | Gets the section view of this section cut. |
| ![ Method](dotnetimages/Method.gif) | [IGetTextFormat](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~IGetTextFormat.html) | Gets the text format for the text for this section line. |
| ![ Method](dotnetimages/Method.gif) | [IGetTextInfo](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~IGetTextInfo.html) | Gets the location of the section line text. |
| ![ Method](dotnetimages/Method.gif) | [IGetView](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~IGetView.html) | Gets the drawing view where the section line appears. |
| ![ Method](dotnetimages/Method.gif) | [IsAligned](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~IsAligned.html) | Gets whether this is an aligned section view. |
| ![ Method](dotnetimages/Method.gif) | [ISetExcludedComponents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~ISetExcludedComponents.html) | Excludes the specified components from this section view. |
| ![ Method](dotnetimages/Method.gif) | [ISetLineInfo](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~ISetLineInfo.html) | Sets the location (both position and arrow heads) of the section line. |
| ![ Method](dotnetimages/Method.gif) | [ISetTextFormat](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~ISetTextFormat.html) | Sets the text format for the text for this section line. |
| ![ Method](dotnetimages/Method.gif) | [SetAutoHatch](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~SetAutoHatch.html) | Sets whether auto hatching is enabled for the section view resulting from this section cut. |
| ![ Method](dotnetimages/Method.gif) | [SetDisplayOnlySpeedPakBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~SetDisplayOnlySpeedPakBodies.html) | Sets whether to display in this section view only the bodies included in the SpeedPak configuration. |
| ![ Method](dotnetimages/Method.gif) | [SetDisplayOnlySurfaceCut](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~SetDisplayOnlySurfaceCut.html) | Sets whether to display only the surface cut by the section line. |
| ![ Method](dotnetimages/Method.gif) | [SetDontCutAllInstances](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~SetDontCutAllInstances.html) | Sets whether all instances of the specified component are uncut in this section view or only in the specified component. |
| ![ Method](dotnetimages/Method.gif) | [SetExcludedComponents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~SetExcludedComponents.html) | Excludes the specified components from this section view. |
| ![ Method](dotnetimages/Method.gif) | [SetLabel](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~SetLabel.html) | Obsolete. Superseded by [IDrSection::ISetLabel2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDrSection~SetLabel2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetLabel2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~SetLabel2.html) | Sets the label for this section view. |
| ![ Method](dotnetimages/Method.gif) | [SetLineInfo](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~SetLineInfo.html) | Sets the location (both position and arrow heads) of the section line. |
| ![ Method](dotnetimages/Method.gif) | [SetPartialSection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~SetPartialSection.html) | Sets whether this is a partial section cut. |
| ![ Method](dotnetimages/Method.gif) | [SetReversedCutDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~SetReversedCutDirection.html) | Sets whether the section cut direction is reversed from the default. |
| ![ Method](dotnetimages/Method.gif) | [SetScaleWithModelChanges](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~SetScaleWithModelChanges.html) | Sets whether the section line scales with changes to the model. |
| ![ Method](dotnetimages/Method.gif) | [SetTextFormat](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection~SetTextFormat.html) | Sets the text format for the text for this section line. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IDrSection Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDrSection.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IEnumDrSections Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEnumDrSections.html)

[ISectionViewData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISectionViewData.html)