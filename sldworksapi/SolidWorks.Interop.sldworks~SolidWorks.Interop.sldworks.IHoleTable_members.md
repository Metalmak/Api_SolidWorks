<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IHoleTable Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IHoleTable Interface |

The following tables list the members exposed by [IHoleTable](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [CombineSameSize](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~CombineSameSize.html) | Gets or sets whether to merge cells of the same size in this hole table. |
| ![ Property](dotnetimages/Property.gif) | [CombineTags](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~CombineTags.html) | Gets or sets whether to combine tags for same-size holes. |
| ![ Property](dotnetimages/Property.gif) | [DatumOrigin](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~DatumOrigin.html) | Gets the datum origin annotation for this hole table. |
| ![ Property](dotnetimages/Property.gif) | [EnableUpdate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~EnableUpdate.html) | Gets or sets whether to update hole table and graphics after [changing hole tags](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IHoleTable~HoleTag.html). |
| ![ Property](dotnetimages/Property.gif) | [HoleCentersVisible](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~HoleCentersVisible.html) | Gets or sets whether to show the hole center marks for this hole table. |
| ![ Property](dotnetimages/Property.gif) | [HoleTag](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~HoleTag.html) | Gets or sets the name of the specified tag in a hole table. |
| ![ Property](dotnetimages/Property.gif) | [HoleTagsVisible](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~HoleTagsVisible.html) | Gets whether the hole tags are visible for this hole table. |
| ![ Property](dotnetimages/Property.gif) | [ShowANSIInchLetterNumberDrillSizes](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~ShowANSIInchLetterNumberDrillSizes.html) | Gets or sets whether to display hole sizes in this hole table using ANSI inch letters and drill numbers. |
| ![ Property](dotnetimages/Property.gif) | [StartingValue](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~StartingValue.html) | Gets or sets the starting value for the datum tags of this hole table. |
| ![ Property](dotnetimages/Property.gif) | [TagStyle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~TagStyle.html) | Gets or sets the tag style for this hole table. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AddHole](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~AddHole.html) | Adds holes to this hole table. |
| ![ Method](dotnetimages/Method.gif) | [AssignTagPrefix](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~AssignTagPrefix.html) | Prefixes the manual datum tags of specified holes with specified text. |
| ![ Method](dotnetimages/Method.gif) | [GetFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~GetFeature.html) | Gets the [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object for this hole table. |
| ![ Method](dotnetimages/Method.gif) | [GetHoleLocationPrecision](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~GetHoleLocationPrecision.html) | Gets the precision to use for location values for this hole table. |
| ![ Method](dotnetimages/Method.gif) | [GetHoleLocationUseDocPrecision](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~GetHoleLocationUseDocPrecision.html) | Gets whether to display the location of this hole table using the document's location precision. |
| ![ Method](dotnetimages/Method.gif) | [GetTableAnnotationCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~GetTableAnnotationCount.html) | Gets the number of hole table annotations for this hole table. |
| ![ Method](dotnetimages/Method.gif) | [GetTableAnnotations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~GetTableAnnotations.html) | Gets the hole table annotations for this hole table feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetTableAnnotations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~IGetTableAnnotations.html) | Gets the hole table annotations for this hole table feature. |
| ![ Method](dotnetimages/Method.gif) | [SetHoleLocationPrecision](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable~SetHoleLocationPrecision.html) | Sets the precision to use for location values for this hole table. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IHoleTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTable.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IHoleTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHoleTableAnnotation.html)

[ITableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITableAnnotation.html)