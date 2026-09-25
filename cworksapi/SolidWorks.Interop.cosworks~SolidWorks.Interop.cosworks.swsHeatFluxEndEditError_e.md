<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsHeatFluxEndEditError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsHeatFluxEndEditError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsHeatFluxEndEditError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Heat flux editing errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsHeatFluxEndEditError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsHeatFluxEndEditError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsHeatFluxEndEditError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsHeatFluxEndEditError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsHeatFluxEndEditErrorEntityAlreadyExists** | 2 = At least one entity is specified more than once |
| **swsHeatFluxEndEditErrorLowerboundTemperatureHigherThanUpperbound** | 7 = Lower-bound temperature must be lower than upper-bound temperature |
| **swsHeatFluxEndEditErrorNoEntities** | 3 = No entities specified |
| **swsHeatFluxEndEditErrorNoEntityAtIndex** | 1 = No entity passed at index |
| **swsHeatFluxEndEditErrorSelectFace** | 4 = Select a face |
| **swsHeatFluxEndEditErrorSelectFacesOrShellEdge** | 5 = Select a fade or shell edge |
| **swsHeatFluxEndEditErrorSelectrVertexForSensorLocation** | 6 = Select a vertex for the location of the sensor |
| **swsHeatFluxEndEditErrorSuccessful** | 0 = Successful |
| **swsHeatFluxEndEditErrorThermostatForTransientStudiesOnly** | 8 = Thermostat is allowed for transient studies only (not allowed for steady-state thermal studies) |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)