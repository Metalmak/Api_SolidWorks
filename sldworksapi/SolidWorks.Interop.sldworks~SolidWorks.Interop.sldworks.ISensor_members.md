<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISensor_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISensor Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ISensor Interface |

The following tables list the members exposed by [ISensor](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISensor.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [SensorAlertEnabled](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISensor~SensorAlertEnabled.html) | Gets or sets whether an alert is triggered when the limits of the sensor deviate from its specified values. |
| ![ Property](dotnetimages/Property.gif) | [SensorAlertState](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISensor~SensorAlertState.html) | Gets whether an alert is currently triggered for this sensor. |
| ![ Property](dotnetimages/Property.gif) | [SensorAlertType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISensor~SensorAlertType.html) | Gets or sets the type of alert for this sensor. |
| ![ Property](dotnetimages/Property.gif) | [SensorAlertValue1](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISensor~SensorAlertValue1.html) | Gets or sets the alert value for this sensor. |
| ![ Property](dotnetimages/Property.gif) | [SensorAlertValue2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISensor~SensorAlertValue2.html) | Gets or sets alert value for this sensor; only in effect when [sensor alert type](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISensor~SensorAlertType.html) set to swSensorAlert\_Between. |
| ![ Property](dotnetimages/Property.gif) | [SensorType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISensor~SensorType.html) | Gets the type of this sensor. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [GetSensorFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISensor~GetSensorFeatureData.html) | Gets a sensor feature data. |
| ![ Method](dotnetimages/Method.gif) | [GetSensorValue](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISensor~GetSensorValue.html) | Gets the value and units of this sensor. |
| ![ Method](dotnetimages/Method.gif) | [UpdateSensor](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISensor~UpdateSensor.html) | Updates the sensor. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ISensor Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISensor.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IDimensionSensorData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDimensionSensorData.html)

[DPartDocEvents\_SensorAlertPreNotifyEventHandler Delegate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DPartDocEvents_SensorAlertPreNotifyEventHandler.html)

[DAssemblyDocEvents\_SensorAlertPreNotifyEventHandler Delegate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DAssemblyDocEvents_SensorAlertPreNotifyEventHandler.html)