<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IDesignTable Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IDesignTable Interface |

The following tables list the members exposed by [IDesignTable](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [AutoAddNewConfigs](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~AutoAddNewConfigs.html) | Gets or sets whether to automatically add rows or columns to the design table when new configurations are added to the model. |
| ![ Property](dotnetimages/Property.gif) | [AutoAddNewParams](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~AutoAddNewParams.html) | Gets or sets whether or not to automatically add rows or columns to the design table when new parameters are added to the model. |
| ![ Property](dotnetimages/Property.gif) | [ColumnHidden](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~ColumnHidden.html) | Gets the visibility state of the specified column. |
| ![ Property](dotnetimages/Property.gif) | [EnableCellDropdownLists](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~EnableCellDropdownLists.html) | Gets or sets whether to enable cell drop-down lists in the design table. |
| ![ Property](dotnetimages/Property.gif) | [FileName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~FileName.html) | Gets or sets the Microsoft Excel file for this design table. |
| ![ Property](dotnetimages/Property.gif) | [LastError](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~LastError.html) | Gets or sets the last error that occurred in this design table. |
| ![ Property](dotnetimages/Property.gif) | [LinkToFile](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~LinkToFile.html) | Gets or sets whether to link the design table to the model. |
| ![ Property](dotnetimages/Property.gif) | [RowHidden](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~RowHidden.html) | Gets the visibility state of the specified row. |
| ![ Property](dotnetimages/Property.gif) | [SourceType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~SourceType.html) | Gets or sets the type of source file for this design table. |
| ![ Property](dotnetimages/Property.gif) | [Updatable](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~Updatable.html) | Gets or sets whether edits to the model update the design table. |
| ![ Property](dotnetimages/Property.gif) | [Warn](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~Warn.html) | Gets or sets whether to display a warning when invalid information is encountered in the design table when updating the design table. |
| ![ Property](dotnetimages/Property.gif) | [Worksheet](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~Worksheet.html) | Gets the Microsoft Excel worksheet for this design table. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AddRow](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~AddRow.html) | Adds a row to the design table. |
| ![ Method](dotnetimages/Method.gif) | [Attach](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~Attach.html) | Activates the design table within the part or assembly document. |
| ![ Method](dotnetimages/Method.gif) | [Detach](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~Detach.html) | Detaches the design table from the Microsoft Excel sheet. |
| ![ Method](dotnetimages/Method.gif) | [EditFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~EditFeature.html) | Lets you change the characteristics of the design table. |
| ![ Method](dotnetimages/Method.gif) | [EditTable](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~EditTable.html) | Obsolete. Superseded by [IDesignTable::EditTable2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDesignTable~EditTable2.html). |
| ![ Method](dotnetimages/Method.gif) | [EditTable2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~EditTable2.html) | Lets you edit the design table. |
| ![ Method](dotnetimages/Method.gif) | [GetColumnCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~GetColumnCount.html) | Gets the number of columns in the design table that are currently visible in the model view. |
| ![ Method](dotnetimages/Method.gif) | [GetEntryText](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~GetEntryText.html) | Gets the contents of the specified cell as a string regardless of the cell's data type. |
| ![ Method](dotnetimages/Method.gif) | [GetEntryValue](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~GetEntryValue.html) | Gets the contents of the specified cell. |
| ![ Method](dotnetimages/Method.gif) | [GetHeaderText](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~GetHeaderText.html) | Gets the header text for the specified column. |
| ![ Method](dotnetimages/Method.gif) | [GetRowCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~GetRowCount.html) | Gets the number of rows in the design table that are currently visible in the model view. |
| ![ Method](dotnetimages/Method.gif) | [GetStartColumnNumber](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~GetStartColumnNumber.html) | Gets the number of the first column in which a dimension is displayed. |
| ![ Method](dotnetimages/Method.gif) | [GetStartRowNumber](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~GetStartRowNumber.html) | Gets the number of the first row in which dimensions are displayed. |
| ![ Method](dotnetimages/Method.gif) | [GetTitle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~GetTitle.html) | Gets the design table title. |
| ![ Method](dotnetimages/Method.gif) | [GetTotalColumnCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~GetTotalColumnCount.html) | Gets the number of columns in the design table. |
| ![ Method](dotnetimages/Method.gif) | [GetTotalRowCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~GetTotalRowCount.html) | Gets the number of rows in the design table. |
| ![ Method](dotnetimages/Method.gif) | [GetVisibleColumnCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~GetVisibleColumnCount.html) | Gets the number of columns visible in this design table. |
| ![ Method](dotnetimages/Method.gif) | [GetVisibleLeftColumnNumber](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~GetVisibleLeftColumnNumber.html) | Gets the number of the leftmost visible column. |
| ![ Method](dotnetimages/Method.gif) | [GetVisibleRowCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~GetVisibleRowCount.html) | Gets the number of rows visible in the design table. |
| ![ Method](dotnetimages/Method.gif) | [GetVisibleTopRowNumber](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~GetVisibleTopRowNumber.html) | Gets the number of the topmost visible row. |
| ![ Method](dotnetimages/Method.gif) | [IsActive](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~IsActive.html) | Gets whether the design table is currently being edited. |
| ![ Method](dotnetimages/Method.gif) | [SaveAsExcelFile](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~SaveAsExcelFile.html) | Saves the design table to a Microsoft Excel file. |
| ![ Method](dotnetimages/Method.gif) | [SetEntryText](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~SetEntryText.html) | Sets the text value of the specified entry. |
| ![ Method](dotnetimages/Method.gif) | [SetEntryValue](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~SetEntryValue.html) | Sets the data type and value in the specified cell. |
| ![ Method](dotnetimages/Method.gif) | [SetRowChanged](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~SetRowChanged.html) | Sets the number of the row that was changed. |
| ![ Method](dotnetimages/Method.gif) | [UpdateFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~UpdateFeature.html) | Updates the characteristics of the design table. |
| ![ Method](dotnetimages/Method.gif) | [UpdateModel](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~UpdateModel.html) | Applies the edits to the design table to the model. |
| ![ Method](dotnetimages/Method.gif) | [UpdateTable](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable~UpdateTable.html) | Applies the changes made to the design table to the model. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IDesignTable Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDesignTable.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)