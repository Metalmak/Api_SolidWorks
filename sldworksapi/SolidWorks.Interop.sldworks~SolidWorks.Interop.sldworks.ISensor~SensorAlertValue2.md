<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISensor~SensorAlertValue2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SensorAlertValue2 Property (ISensor) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISensor Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISensor.html) : SensorAlertValue2 Property (ISensor) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets alert value for this sensor; only in effect when [sensor alert type](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISensor~SensorAlertType.html) set to swSensorAlert\_Between.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property SensorAlertValue2 As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISensor Dim value As System.Double   instance.SensorAlertValue2 = value   value = instance.SensorAlertValue2 ``` | |

| C# |  |
| --- | --- |
| ``` System.double SensorAlertValue2 {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double SensorAlertValue2 {    System.double get();    void set ( &   System.double value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Alert value

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sensor::SensorAlertValue2.

# ![](dotnetimages/collapse.gif)Example

[Get and Set Sensor (C#)](Get_and_Set_Sensor_Example_CSharp.htm)

[Get and Set Sensor (VB.NET)](Get_and_Set_Sensor_Example_VBNET.htm)

[Get and Set Sensor (VBA)](Get_and_Set_Sensor_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISensor Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISensor.html)

[ISensor Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISensor_members.html)

[ISensor::SensorAlertValue1 Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISensor~SensorAlertValue1.html)

[ISensor::SensorAlertState Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISensor~SensorAlertState.html)

[ISensor::SensorAlertEnabled Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISensor~SensorAlertEnabled.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 SP2, Revision Number 17.2