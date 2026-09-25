<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IMacroFeatureData Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IMacroFeatureData Interface |

The following tables list the members exposed by [IMacroFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [CurrentConfiguration](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~CurrentConfiguration.html) | Gets the macro feature configuration being rebuilt. |
| ![ Property](dotnetimages/Property.gif) | [EditBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~EditBodies.html) | Gets or sets the bodies to be modified by this macro feature. |
| ![ Property](dotnetimages/Property.gif) | [EditBody](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~EditBody.html) | Obsolete. Superseded by [IMacroFeatureData::IGetEditBodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMacroFeatureData~IGetEditBodies.html), [IMacroFeatureData::ISetEditBodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMacroFeatureData~ISetEditBodies.html), and [IMacroFeatureData::EditBodies](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMacroFeatureData~EditBodies.html). |
| ![ Property](dotnetimages/Property.gif) | [EnableMultiBodyConsume](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~EnableMultiBodyConsume.html) | Gets or sets whether to replace the original edit body with multiple solid bodies created during regeneration of a multibody macro feature. |
| ![ Property](dotnetimages/Property.gif) | [FeatureTransform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~FeatureTransform.html) | Gets and sets the macro feature transform. |
| ![ Property](dotnetimages/Property.gif) | [IconFiles](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IconFiles.html) | Gets or sets the file names for the icons for this macro feature. |
| ![ Property](dotnetimages/Property.gif) | [MacroFileEmbedded](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~MacroFileEmbedded.html) | Gets whether the macro file is embedded ini the model with the macro feature. |
| ![ Property](dotnetimages/Property.gif) | [MacroFileName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~MacroFileName.html) | Gets or sets the path and file name for the macro for the macro feature. |
| ![ Property](dotnetimages/Property.gif) | [ModuleName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~ModuleName.html) | Gets or sets the name of a module in the macro for this macro feature. |
| ![ Property](dotnetimages/Property.gif) | [Parents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~Parents.html) | Gets or sets the parent features for this macro feature. |
| ![ Property](dotnetimages/Property.gif) | [PatternTransform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~PatternTransform.html) | Gets the pattern transform. |
| ![ Property](dotnetimages/Property.gif) | [ProcedureName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~ProcedureName.html) | Gets or sets a name of the procedure in the macro for this macro feature. |
| ![ Property](dotnetimages/Property.gif) | [PropertyManagerHandleMacroFileName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~PropertyManagerHandleMacroFileName.html) | Gets or sets the path and file name for the macro file from or to the PropertyManager handle for this macro feature. |
| ![ Property](dotnetimages/Property.gif) | [PropertyManagerHandleModuleName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~PropertyManagerHandleModuleName.html) | Gets or sets the name of the module in the macro file from or to the PropertyManager handle. |
| ![ Property](dotnetimages/Property.gif) | [PropertyManagerHandleProcedureName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~PropertyManagerHandleProcedureName.html) | Gets or sets the name of the procedure in the macro file from or to the PropertyManager handle. |
| ![ Property](dotnetimages/Property.gif) | [Provider](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~Provider.html) | Gets or sets the error message to display in the What's Wrong dialog when a non-embedded macro feature fails to rebuild due to missing files. |
| ![ Property](dotnetimages/Property.gif) | [SecurityHandleMacroFileName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~SecurityHandleMacroFileName.html) | Gets or sets the name of the procedure in the macro file from or to the security handle. |
| ![ Property](dotnetimages/Property.gif) | [SecurityHandleModuleName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~SecurityHandleModuleName.html) | Gets and sets the name of the module in the macro file from or to the security handle. |
| ![ Property](dotnetimages/Property.gif) | [SecurityHandleProcedureName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~SecurityHandleProcedureName.html) | Gets or sets the name of the procedure in the macro file from or to the security handle. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~AccessSelections.html) | Gains access to the selections associated with this macro feature. |
| ![ Method](dotnetimages/Method.gif) | [EmbedMacroFile](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~EmbedMacroFile.html) | Sets whether to embed the macro file in the model with the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetBaseName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetBaseName.html) | Gets the name of the base feature for this macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetDisplayDimensionCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetDisplayDimensionCount.html) | Gets the number of display dimensions for this macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetDisplayDimensions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetDisplayDimensions.html) | Gets the display dimensions for this macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetDoubleByName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetDoubleByName.html) | Gets a double value by parameter name. |
| ![ Method](dotnetimages/Method.gif) | [GetEdgeIdType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetEdgeIdType.html) | Gets the ID type of the specified edge for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetEdgeUserId](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetEdgeUserId.html) | Gets the user-defined IDs for the specified edge for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetEditBodiesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetEditBodiesCount.html) | Gets the number of bodies to be modified by this macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetEditTargetTransform](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetEditTargetTransform.html) | Gets the transform of the component where the macro feature resides if at least one selection in the macro feature belongs to a different component. |
| ![ Method](dotnetimages/Method.gif) | [GetEntitiesNeedUserId](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetEntitiesNeedUserId.html) | Gets a list of faces and edges that need be assigned user IDs for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetEntitiesNeedUserIdCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetEntitiesNeedUserIdCount.html) | Gets the number of faces and edges that need to be assigned user IDs for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetFaceIdType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetFaceIdType.html) | Gets the ID type from the face for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetFaceUserId](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetFaceUserId.html) | Gets the user-defined IDs for the specified face. |
| ![ Method](dotnetimages/Method.gif) | [GetIconFileCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetIconFileCount.html) | Gets the number of the files for the icons for this macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetIntegerByName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetIntegerByName.html) | Gets an integer value by parameter name. |
| ![ Method](dotnetimages/Method.gif) | [GetModuleCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetModuleCount.html) | Gets the number of modules for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetModuleNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetModuleNames.html) | Gets the names of the modules in the macro for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetParameterCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetParameterCount.html) | Gets the number of user-defined parameters. |
| ![ Method](dotnetimages/Method.gif) | [GetParameters](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetParameters.html) | Gets the user-defined parameters. |
| ![ Method](dotnetimages/Method.gif) | [GetParentsCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetParentsCount.html) | Gets the number of parent features for this macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetProcedureCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetProcedureCount.html) | Gets the number of procedures in the specified module in the macro for this macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetProcedureNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetProcedureNames.html) | Gets the names of the procedures in the specified module for the macro for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetProgId](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetProgId.html) | Gets the version-independent program ID that is valid for this COM feature. |
| ![ Method](dotnetimages/Method.gif) | [GetPropertyManagerHandleModuleCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetPropertyManagerHandleModuleCount.html) | Gets the number of modules in the macro from the PropertyManager handle for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetPropertyManagerHandleModuleNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetPropertyManagerHandleModuleNames.html) | Gets the names of the modules in the macro from the PropertyManager handle for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetPropertyManagerHandleProcedureCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetPropertyManagerHandleProcedureCount.html) | Gets the number of procedures in the specified module in the macro from the PropertyManager handle for this macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetPropertyManagerHandleProcedureNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetPropertyManagerHandleProcedureNames.html) | Gets the names of the procedures in the specified module in the macro from the PropertyManager handle for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetSelectionCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetSelectionCount.html) | Gets the number of selected objects for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetSelections.html) | Obsolete. Superseded by [IMacroFeatureData::GetSelections3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMacroFeatureData~IGetSelections3.html). |
| ![ Method](dotnetimages/Method.gif) | [GetSelections2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetSelections2.html) | Obsolete. Superseded by [IMacroFeatureData::GetSelections3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMacroFeatureData~GetSelections3.html). |
| ![ Method](dotnetimages/Method.gif) | [GetSelections3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetSelections3.html) | Gets the selected objects for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [GetStringByName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~GetStringByName.html) | Gets a string value by the name of the parameter for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [IAccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IAccessSelections.html) | Gains access to the selections associated with this macro feature. |
| ![ Method](dotnetimages/Method.gif) | [IAddDisplayDimensions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IAddDisplayDimensions.html) | Adds the specified display dimensions to this macro feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetDisplayDimensions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IGetDisplayDimensions.html) | Gets the display dimensions for this macro feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetEditBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IGetEditBodies.html) | Gets the bodies to be modified by this macro feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetEntitiesNeedUserId](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IGetEntitiesNeedUserId.html) | Gets a list of faces and edges that need be assigned user IDs for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetIconFiles](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IGetIconFiles.html) | Gets the file names for the icons for this macro feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetModuleNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IGetModuleNames.html) | Gets the names of the modules in the macro for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetParameters](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IGetParameters.html) | Gets the user-defined parameters. |
| ![ Method](dotnetimages/Method.gif) | [IGetParents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IGetParents.html) | Gets the parent features of this macro feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetProcedureNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IGetProcedureNames.html) | Gets the names of the procedures in the specified module in the macro for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetPropertyManagerHandleModuleNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IGetPropertyManagerHandleModuleNames.html) | Gets the names of the modules in the macro from the PropertyManager handle for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetPropertyManagerHandleProcedureNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IGetPropertyManagerHandleProcedureNames.html) | Gets the names of the procedures in the specified module in the macro from the PropertyManager handle for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [IGetSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IGetSelections.html) | Obsolete. Superseded by [IMacroFeatureData::IGetSelections3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMacroFeatureData~IGetSelections3.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetSelections2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IGetSelections2.html) | Obsolete. Superseded by [IMacroFeatureData::IGetSelections3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMacroFeatureData~IGetSelections3.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetSelections3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IGetSelections3.html) | Gets the selected objects for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [IsCOMFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~IsCOMFeature.html) | Gets whether the feature is a COM feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetEditBodies](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~ISetEditBodies.html) | Sets the bodies to be modified by this macro feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetIconFiles](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~ISetIconFiles.html) | Sets the file names for the icons for this macro feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetParameters](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~ISetParameters.html) | Sets the user-defined parameters. |
| ![ Method](dotnetimages/Method.gif) | [ISetParents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~ISetParents.html) | Sets the parent features for this macro feature. |
| ![ Method](dotnetimages/Method.gif) | [ISetSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~ISetSelections.html) | Obsolete. Superseded by [IMacroFeatureData::ISetSelections2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMacroFeatureData~ISetSelections2.html). |
| ![ Method](dotnetimages/Method.gif) | [ISetSelections2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~ISetSelections2.html) | Sets the selected objects for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~ReleaseSelectionAccess.html) | Releases access to the selections associated with this macro feature. |
| ![ Method](dotnetimages/Method.gif) | [SetDoubleByName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~SetDoubleByName.html) | Sets a double value by parameter name for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [SetEdgeUserId](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~SetEdgeUserId.html) | Sets the user-defined IDs for the specified edge for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [SetFaceUserId](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~SetFaceUserId.html) | Sets user-defined IDs for the face for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [SetIntegerByName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~SetIntegerByName.html) | Sets an integer value by parameter name. |
| ![ Method](dotnetimages/Method.gif) | [SetParameters](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~SetParameters.html) | Sets the user-defined parameters. |
| ![ Method](dotnetimages/Method.gif) | [SetProgId](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~SetProgId.html) | Sets the version-independent program ID that is valid for this COM feature. |
| ![ Method](dotnetimages/Method.gif) | [SetSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~SetSelections.html) | Obsolete. Superseded by [IMacroFeatureData::SetSelections2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMacroFeatureData~SetSelections2.html). |
| ![ Method](dotnetimages/Method.gif) | [SetSelections2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~SetSelections2.html) | Sets the selected objects for the macro feature. |
| ![ Method](dotnetimages/Method.gif) | [SetStringByName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData~SetStringByName.html) | Sets a string value by parameter name. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IMacroFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMacroFeatureData.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IFeatureManager::IInsertMacroFeature3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~IInsertMacroFeature3.html)

[IFeatureManager::InsertMacroFeature3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMacroFeature3.html)