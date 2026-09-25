<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IDimension Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IDimension Interface |

The following tables list the members exposed by [IDimension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [DimensionLineDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~DimensionLineDirection.html) | Gets or sets the direction of this dimension line. |
| ![ Property](dotnetimages/Property.gif) | [DrivenState](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~DrivenState.html) | Gets or sets the driven state of a dimension. |
| ![ Property](dotnetimages/Property.gif) | [ExtensionLineDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~ExtensionLineDirection.html) | Gets or sets the direction of the extension line. |
| ![ Property](dotnetimages/Property.gif) | [FullName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~FullName.html) | Gets the full name of a dimension including the feature and the model. |
| ![ Property](dotnetimages/Property.gif) | [Name](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~Name.html) | Gets or sets the name of a dimension. |
| ![ Property](dotnetimages/Property.gif) | [ReadOnly](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~ReadOnly.html) | Gets or sets the read-only state of a dimension. |
| ![ Property](dotnetimages/Property.gif) | [ReferencePoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~ReferencePoints.html) | Gets or sets the reference points for this dimension. |
| ![ Property](dotnetimages/Property.gif) | [SystemValue](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~SystemValue.html) | Obsolete. Superseded by [IDimension::GetSystemValue3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~GetSystemValue3.html), [IDimension::IGetSystemValue3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~IGetSystemValue3.html), [IDimension::SetSystemValue3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~SetSystemValue3.html), and [IDimension::ISetSystemValue3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~ISetSystemValue3.html). |
| ![ Property](dotnetimages/Property.gif) | [Tolerance](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~Tolerance.html) | Gets the [IDimensionTolerance](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance.html) object. |
| ![ Property](dotnetimages/Property.gif) | [Value](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~Value.html) | Obsolete. Superseded by [IDimension::GetValue3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~GetValue3.html), [IDimension::IGetValue3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~IGetValue3.html), [IDimension::ISetValue3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~ISetValue3.html), and [IDimension::SetValue3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~SetValue3.html). |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [GetArcEndCondition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~GetArcEndCondition.html) | Gets the end conditions for linear dimensions that end on an arc. |
| ![ Method](dotnetimages/Method.gif) | [GetFeatureOwner](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~GetFeatureOwner.html) | Gets the feature for this dimension. |
| ![ Method](dotnetimages/Method.gif) | [GetNameForSelection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~GetNameForSelection.html) | Gets the name of the selected dimension needed by [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetReferencePointsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~GetReferencePointsCount.html) | Gets the number of reference points for this dimension. |
| ![ Method](dotnetimages/Method.gif) | [GetSystemChamferValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~GetSystemChamferValues.html) | Gets the chamfer dimension values in system units. |
| ![ Method](dotnetimages/Method.gif) | [GetSystemValue2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~GetSystemValue2.html) | Obsolete. See [IDimension::GetSystemValue3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~GetSystemValue3.html) and [IDimension::IGetSystemValue3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~IGetSystemValue3.html). |
| ![ Method](dotnetimages/Method.gif) | [GetSystemValue3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~GetSystemValue3.html) | Gets the value of the current dimension in system units in the named configuration. |
| ![ Method](dotnetimages/Method.gif) | [GetToleranceFitValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~GetToleranceFitValues.html) | Obsolete. Superseded by [IDimensionTolerance::GetHoleFitValue](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~GetHoleFitValue.html) and [IDimensionTolerance::GetShaftFitValue](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~GetShaftFitValue.html). |
| ![ Method](dotnetimages/Method.gif) | [GetToleranceFontInfo](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~GetToleranceFontInfo.html) | Obsolete. Superseded by [IDimensionTolerance::GetFontUseDimension](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~GetFitFontUseDimension.html), [IDimensionTolerance::GetFontUseScale](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~GetFitFontUseScale.html), [IDimensionTolerance::GetFontScale](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~GetFontScale.html), and [IDimensionTolerance::GetFontHeight](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~GetFontHeight.html). |
| ![ Method](dotnetimages/Method.gif) | [GetToleranceType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~GetToleranceType.html) | Obsolete. Superseded by [IDimensionTolerance::Type](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~Type.html). |
| ![ Method](dotnetimages/Method.gif) | [GetToleranceValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~GetToleranceValues.html) | Obsolete. Superseded by [IDimensionTolerance::GetMaxValue](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~GetMaxValue.html) and [IDimensionTolerance::GetMinValue](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~GetMinValue.html). |
| ![ Method](dotnetimages/Method.gif) | [GetType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~GetType.html) | Gets the type of dimension. |
| ![ Method](dotnetimages/Method.gif) | [GetUserValueIn](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~GetUserValueIn.html) | Gets the value of this dimension in the units of the specified document. |
| ![ Method](dotnetimages/Method.gif) | [GetValue2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~GetValue2.html) | Obsolete. Superseded by [IDimension::GetValue3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~GetValue3.html) and [IDimension::IGetValue3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~IGetValue3.html). |
| ![ Method](dotnetimages/Method.gif) | [GetValue3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~GetValue3.html) | Gets the values of the dimensions in the specified configurations. |
| ![ Method](dotnetimages/Method.gif) | [IGetReferencePoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~IGetReferencePoints.html) | Gets the reference points for this dimension. |
| ![ Method](dotnetimages/Method.gif) | [IGetSystemValue3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~IGetSystemValue3.html) | Gets the value of the current dimension in system units in the named configuration. |
| ![ Method](dotnetimages/Method.gif) | [IGetToleranceFontInfo](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~IGetToleranceFontInfo.html) | Obsolete. Superseded by [IDimensionTolerance::GetFontUseDimension](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~GetFitFontUseDimension.html), [IDimensionTolerance::GetFontUseScale](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~GetFitFontUseScale.html), [IDimensionTolerance::GetFontScale](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~GetFontScale.html), and [IDimensionTolerance::GetFontHeight](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~GetFontHeight.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetToleranceValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~IGetToleranceValues.html) | Obsolete. Superseded by [IDimensionTolerance::GetMaxValue](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~GetMaxValue.html) and [IDimensionTolerance::GetMinValue](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~GetMinValue.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetUserValueIn](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~IGetUserValueIn.html) | Obsolete. Superseded by [IDimension::IGetUserValueIn2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~IGetUserValueIn2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetUserValueIn2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~IGetUserValueIn2.html) | Gets the value of this dimension in the units of the specified document. |
| ![ Method](dotnetimages/Method.gif) | [IGetValue3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~IGetValue3.html) | Gets the values of the dimensions in the specified configurations. |
| ![ Method](dotnetimages/Method.gif) | [IsAppliedToAllConfigurations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~IsAppliedToAllConfigurations.html) | Gets whether a dimension is currently applied to all configurations of the model or to just the current configuration. |
| ![ Method](dotnetimages/Method.gif) | [IsDesignTableDimension](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~IsDesignTableDimension.html) | Gets whether this dimension is driven by a design table. |
| ![ Method](dotnetimages/Method.gif) | [ISetReferencePoints](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~ISetReferencePoints.html) | Sets the reference points for this dimension. |
| ![ Method](dotnetimages/Method.gif) | [ISetSystemValue3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~ISetSystemValue3.html) | Sets the value of this dimension in system units (meters) in the specified configuration. |
| ![ Method](dotnetimages/Method.gif) | [ISetUserValueIn](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~ISetUserValueIn.html) | Obsolete. Superseded by [IDimension::ISetUserValueIn3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~ISetUserValueIn3.html). |
| ![ Method](dotnetimages/Method.gif) | [ISetUserValueIn2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~ISetUserValueIn2.html) | Obsolete. Superseded by [IDimension::ISetUserValueIn3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~ISetUserValueIn3.html). |
| ![ Method](dotnetimages/Method.gif) | [ISetUserValueIn3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~ISetUserValueIn3.html) | Sets the value of this dimension in the units of the specified document. |
| ![ Method](dotnetimages/Method.gif) | [ISetValue3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~ISetValue3.html) | Sets the values of the dimensions in the specified configurations. |
| ![ Method](dotnetimages/Method.gif) | [IsReference](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~IsReference.html) | Gets whether the dimension is a reference dimension. |
| ![ Method](dotnetimages/Method.gif) | [SetArcEndCondition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~SetArcEndCondition.html) | Sets the end conditions for linear dimensions that end on an arc. |
| ![ Method](dotnetimages/Method.gif) | [SetSystemValue2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~SetSystemValue2.html) | Obsolete. Superseded by [IDimension::SetSystemValue3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~SetSystemValue3.html). |
| ![ Method](dotnetimages/Method.gif) | [SetSystemValue3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~SetSystemValue3.html) | Sets the value of this dimension in system units (meters) in the specified configuration. |
| ![ Method](dotnetimages/Method.gif) | [SetToleranceFitValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~SetToleranceFitValues.html) | Obsolete. Superseded by [IDimensionTolerance::SetFitValues](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~SetFitValues.html). |
| ![ Method](dotnetimages/Method.gif) | [SetToleranceFontInfo](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~SetToleranceFontInfo.html) | Obsolete. Superseded by [IDimensionTolerance::SetFont](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~SetFont.html). |
| ![ Method](dotnetimages/Method.gif) | [SetToleranceType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~SetToleranceType.html) | Obsolete. Superseded by [IDimensionTolerance::Type](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~Type.html). |
| ![ Method](dotnetimages/Method.gif) | [SetToleranceValues](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~SetToleranceValues.html) | Obsolete. Superseded by [IDimensionTolerance::SetValues](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimensionTolerance~SetValues.html). |
| ![ Method](dotnetimages/Method.gif) | [SetUserValueIn](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~SetUserValueIn.html) | Obsolete. Superseded by [IDimension::SetUserValueIn2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~SetUserValueIn2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetUserValueIn2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~SetUserValueIn2.html) | Sets the value of this dimension in the units of the specified document. |
| ![ Method](dotnetimages/Method.gif) | [SetValue2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~SetValue2.html) | Obsolete. Superseded by [IDimension::SetValue3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDimension~SetValue3.html). |
| ![ Method](dotnetimages/Method.gif) | [SetValue3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension~SetValue3.html) | Sets the values of the dimensions in the specified configurations. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimension.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IDisplayDimension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDisplayDimension.html)

[IDimensionTolerance Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimensionTolerance.html)