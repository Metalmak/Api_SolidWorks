<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsHeatPowerEndEditError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsHeatPowerEndEditError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsHeatPowerEndEditError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Heat power editing errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsHeatPowerEndEditError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsHeatPowerEndEditError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsHeatPowerEndEditError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsHeatPowerEndEditError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsHeatPowerEndEditErrorEntityAlreadyExists** | 2 = At least one entity is specified more than once |
| **swsHeatPowerEndEditErrorLowerboundTemperatureHigherThanUpperbound** | 7 = Lower-bound temperature cannot be higher than the upper-bound temperature |
| **swsHeatPowerEndEditErrorNoEntitiesSelected** | 3 = No entities specified |
| **swsHeatPowerEndEditErrorNoEntityAtIndex** | 1 = No entity passed at index |
| **swsHeatPowerEndEditErrorNotValidForSteadyStateAnalysis** | 8 = Not valid for steady-state analysis; solution type must be transient |
| **swsHeatPowerEndEditErrorSelectFaceEdgeOrVertex** | 5 = Select a face, edge, or vertex |
| **swsHeatPowerEndEditErrorSelectVertexForThermostatLocation** | 6 = Specify a vertex for the location of the thermostat |
| **swsHeatPowerEndEditErrorSelectVerticesEdgesFacesComponentsOrBodies** | 4 = Select vertices, edges, faces, components, or bodies |
| **swsHeatPowerEndEditErrorSuccessful** | 0 = Successful |
| **swsHeatPowerEndEditErrorVertexCannotBeUsedForSensorLocation** | 9 = A vertex in the selected entities cannot be used for the location of the sensor |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)