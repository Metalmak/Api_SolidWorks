<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IEquationMgr Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IEquationMgr Interface |

The following tables list the members exposed by [IEquationMgr](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [AngularEquationUnits](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~AngularEquationUnits.html) | Gets or sets the angular units used in equations. |
| ![ Property](dotnetimages/Property.gif) | [AutomaticRebuild](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~AutomaticRebuild.html) | Gets or sets whether to automatically rebuild after modifications. |
| ![ Property](dotnetimages/Property.gif) | [AutomaticSolveOrder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~AutomaticSolveOrder.html) | Gets or sets whether to automatically sequence equations in an order determined by SOLIDWORKS to produce accurate results. |
| ![ Property](dotnetimages/Property.gif) | [Disabled](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~Disabled.html) | Gets or sets whether to disable the specified equation in the model. |
| ![ Property](dotnetimages/Property.gif) | [Equation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~Equation.html) | Gets or sets the equation at the specified index. |
| ![ Property](dotnetimages/Property.gif) | [FilePath](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~FilePath.html) | Gets or sets the path for an exported equation text (**.txt**) file. |
| ![ Property](dotnetimages/Property.gif) | [GlobalVariable](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~GlobalVariable.html) | Gets whether the equation at the specified index is a global variable. |
| ![ Property](dotnetimages/Property.gif) | [LinkToFile](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~LinkToFile.html) | Gets or sets whether the equation is linked to an exported equation text (**.txt**) file. |
| ![ Property](dotnetimages/Property.gif) | [Status](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~Status.html) | Gets the status of the last equation that was executed. |
| ![ Property](dotnetimages/Property.gif) | [Suppression](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~Suppression.html) | Obsolete as of SOLIDWORKS 2014 and later. |
| ![ Property](dotnetimages/Property.gif) | [Value](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~Value.html) | Gets the value of the equation at the specified index. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [Add](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~Add.html) | Obsolete. Superseded by [IEquationMgr::Add2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEquationMgr~Add2.html). |
| ![ Method](dotnetimages/Method.gif) | [Add2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~Add2.html) | Adds an equation at the specified index. |
| ![ Method](dotnetimages/Method.gif) | [Add3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~Add3.html) | Adds an equation at the specified index for the specified configurations. |
| ![ Method](dotnetimages/Method.gif) | [ChangeSuppressionForAllConfigurations](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~ChangeSuppressionForAllConfigurations.html) | Changes the suppression state of the specified equation in all configurations. |
| ![ Method](dotnetimages/Method.gif) | [ChangeSuppressionForConfiguration](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~ChangeSuppressionForConfiguration.html) | Changes the suppression state of an equation in the specified configuration. |
| ![ Method](dotnetimages/Method.gif) | [Delete](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~Delete.html) | Deletes the equation at the specified index. |
| ![ Method](dotnetimages/Method.gif) | [EvaluateAll](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~EvaluateAll.html) | Evaluates all equations. |
| ![ Method](dotnetimages/Method.gif) | [GetConfigurationOption](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~GetConfigurationOption.html) | Gets the configuration option for the equation at the specified index. |
| ![ Method](dotnetimages/Method.gif) | [GetCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~GetCount.html) | Gets the number of equations in the model. |
| ![ Method](dotnetimages/Method.gif) | [GetDisabledEquationCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~GetDisabledEquationCount.html) | Gets the number of disabled equations in the model. |
| ![ Method](dotnetimages/Method.gif) | [IAdd3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~IAdd3.html) | Adds an equation at the specified index for the specified configurations. |
| ![ Method](dotnetimages/Method.gif) | [ISetEquationAndConfigurationOption](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~ISetEquationAndConfigurationOption.html) | Modifies the equation at the specified index for the specified configurations. |
| ![ Method](dotnetimages/Method.gif) | [SetEquationAndConfigurationOption](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~SetEquationAndConfigurationOption.html) | Modifies the equation at the specified index for the specified configurations. |
| ![ Method](dotnetimages/Method.gif) | [UpdateValuesFromExternalEquationFile](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr~UpdateValuesFromExternalEquationFile.html) | Updates equations dependent on a linked equation file and ensures that the linked equation file exists and updates its current path, if necessary. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IEquationMgr Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEquationMgr.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)