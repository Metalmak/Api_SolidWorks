<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsStudyExportError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsStudyExportError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsStudyExportError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Export study errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsStudyExportError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsStudyExportError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsStudyExportError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsStudyExportError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsStudyExportError\_CreepMaterial** | 4 = Creep material does not have the force control method |
| **swsStudyExportError\_DropTestNotAvailable** | 3 = Drop test parameters are not exported |
| **swsStudyExportError\_LoadOnPointsNotAvailable** | 6 = Export option is not available for load on points |
| **swsStudyExportError\_NoError** | 0 = No error |
| **swsStudyExportError\_OptimizationNotAvailable** | 1 = Export option is not available for an optimization study |
| **swsStudyExportError\_RemoteLoadConnectorNotAvailable** | 5 = Export option is not available with remote load or connector |
| **swsStudyExportError\_TransientThermalNotAvailable** | 2 = Transient thermal analysis does not have an initial temperature |
| **swsStudyExportError\_Wrong\_NastranExportUnit** | 11 = The specified unit is incorrect for the NASTRAN export option |
| **swsStudyExportError\_WrongCosmosExportOption** | 9 = The Cosmos export option is not supported (should not exceed the value of [swsCosmosExportOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsCosmosExportOption_e.html) if study export option [swsStudyExportOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStudyExportOption_e.html).swsStudyExport\_Cosmos is selected) |
| **swsStudyExportError\_WrongCosmosExportOptionForNoMesh** | 8 = Wrong Cosmos export option for no mesh export |
| **swsStudyExportError\_WrongCosmosExportUnit** | 12 = The specified unit is incorrect for GEOSTAR export option |
| **swsStudyExportError\_WrongFileOption** | 7 = The study export option is not supported (should not exceed the value of [swsStudyExportOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStudyExportOption_e.html)) |
| **swsStudyExportError\_WrongNastranExportOption** | 10 = The NASTRAN export option is not supported (should not exceed the value of [swsNastranExportOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsNastranExportOption_e.html) if study export option [swsStudyExportOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStudyExportOption_e.html).swsStudyExport\_Nastran is selected) |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)