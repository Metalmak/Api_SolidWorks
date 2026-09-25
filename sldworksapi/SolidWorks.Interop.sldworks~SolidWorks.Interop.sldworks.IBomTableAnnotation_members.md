<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IBomTableAnnotation Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IBomTableAnnotation Interface |

The following tables list the members exposed by [IBomTableAnnotation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [BomFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~BomFeature.html) | Gets the BOM for this table annotation. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [ApplySavedSortScheme](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~ApplySavedSortScheme.html) | Sorts this BOM table using the sort data that was previously saved in the table. |
| ![ Method](dotnetimages/Method.gif) | [Collapse](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~Collapse.html) | Collapses the specified item. |
| ![ Method](dotnetimages/Method.gif) | [Dissolve](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~Dissolve.html) | Dissolves into individual components the subassembly or weldment at the specified row index of this BOM table annotation. |
| ![ Method](dotnetimages/Method.gif) | [Expand](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~Expand.html) | Expands the specified item. |
| ![ Method](dotnetimages/Method.gif) | [GetAllCustomProperties](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~GetAllCustomProperties.html) | Gets the list of available custom properties that can be used for a custom properties column in this BOM table annotation. |
| ![ Method](dotnetimages/Method.gif) | [GetAllCustomPropertiesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~GetAllCustomPropertiesCount.html) | Gets the number of items in the list of available custom properties that can be used for a custom properties column in this BOM table annotation. |
| ![ Method](dotnetimages/Method.gif) | [GetBomTableSortData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~GetBomTableSortData.html) | Gets an instance of [IBomTableSortData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomTableSortData.html). |
| ![ Method](dotnetimages/Method.gif) | [GetColumnCustomProperty](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~GetColumnCustomProperty.html) | Gets the custom property used to fill the values in a specified user-defined column. |
| ![ Method](dotnetimages/Method.gif) | [GetColumnUseTitleAsPartNumber](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~GetColumnUseTitleAsPartNumber.html) | Gets whether the document title is being used for the specified part-number column. |
| ![ Method](dotnetimages/Method.gif) | [GetComponents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~GetComponents.html) | Obsolete. Superseded by [IBomTableAnnotation::GetComponents2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomTableAnnotation~GetComponents2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetComponents2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~GetComponents2.html) | Gets the components in the specified row for the specified configuration in this BOM table annotation. |
| ![ Method](dotnetimages/Method.gif) | [GetComponentsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~GetComponentsCount.html) | Obsolete. Superseded by [IBomTableAnnotation::GetComponentsCount2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomTableAnnotation~GetComponentsCount2.html). |
| ![ Method](dotnetimages/Method.gif) | [GetComponentsCount2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~GetComponentsCount2.html) | Gets the number of components, the item number, and the part number in the specified row for the specified configuration in this BOM table annotation. |
| ![ Method](dotnetimages/Method.gif) | [GetModelPathNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~GetModelPathNames.html) | Gets the full pathnames of all documents in the specified row of this BOM table annotation. Also gets the item and part numbers associated with the specified row. |
| ![ Method](dotnetimages/Method.gif) | [GetModelPathNamesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~GetModelPathNamesCount.html) | Gets the number of model pathnames in the specified row of this BOM table annotation. |
| ![ Method](dotnetimages/Method.gif) | [IGetAllCustomProperties](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~IGetAllCustomProperties.html) | Gets the list of available custom properties that can be used for a custom properties column in this BOM table annotation. |
| ![ Method](dotnetimages/Method.gif) | [IGetComponents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~IGetComponents.html) | Obsolete. Superseded by [IBomTableAnnotation::IGetComponents2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBomTableAnnotation~IGetComponents2.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetComponents2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~IGetComponents2.html) | Gets the components in the specified row for the specified configuration in this BOM table annotation. |
| ![ Method](dotnetimages/Method.gif) | [IGetModelPathNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~IGetModelPathNames.html) | Gets the full pathnames of all documents in the specified row of this BOM table annotation. Also gets the item and part numbers associated with the specified row. |
| ![ Method](dotnetimages/Method.gif) | [RestoreRestructuredComponents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~RestoreRestructuredComponents.html) | Restores the previously dissolved subassembly or weldment at the specified row index of this BOM table annotation. |
| ![ Method](dotnetimages/Method.gif) | [SaveAsExcel](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~SaveAsExcel.html) | Saves this BOM table annotation as a Microsoft Excel document with the specified properties. |
| ![ Method](dotnetimages/Method.gif) | [SetColumnCustomProperty](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~SetColumnCustomProperty.html) | Sets the custom property used to fill the values in a specified user-defined column. |
| ![ Method](dotnetimages/Method.gif) | [SetColumnUseTitleAsPartNumber](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~SetColumnUseTitleAsPartNumber.html) | Sets whether to use the document title for the specified part-number column. |
| ![ Method](dotnetimages/Method.gif) | [Sort](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation~Sort.html) | Sorts this BOM table using the specified sorting data. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IBomTableAnnotation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableAnnotation.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IBomTableSortData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBomTableSortData.html)