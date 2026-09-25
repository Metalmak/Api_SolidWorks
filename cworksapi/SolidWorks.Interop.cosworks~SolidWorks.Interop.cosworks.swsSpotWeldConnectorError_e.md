<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsSpotWeldConnectorError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsSpotWeldConnectorError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsSpotWeldConnectorError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Spot weld connector errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsSpotWeldConnectorError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsSpotWeldConnectorError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsSpotWeldConnectorError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsSpotWeldConnectorError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **SpotWeldConnectorErrorSelectVerticesOrDatumPoint** | 7 = Select vertices or a datum point |
| **swsSpotWeldConnectorErrorBodyExcludedFromAnalysis** | 16 = Selected entity is on a body excluded from analysis |
| **swsSpotWeldConnectorErrorEmptyArray** | 14 = Array for spot-weld entity is empty |
| **swsSpotWeldConnectorErrorGapTooBig** | 10 = Current gap between the spot-weld faces is greater than the recommended 3 mm |
| **swsSpotWeldConnectorErrorHasRemoteMass** | 15 = Spot-weld connector has a remote mass |
| **swsSpotWeldConnectorErrorInvalidArray** | 13 = Invalid array |
| **swsSpotWeldConnectorErrorInvalidMesh** | 1 = Invalid mesh |
| **swsSpotWeldConnectorErrorInvalidStudy** | 3 = Invalid study |
| **swsSpotWeldConnectorErrorNonlinearStudyPartDocument** | 2 = Study type equals nonlinear and document type equals part |
| **swsSpotWeldConnectorErrorNullDispatch** | 4 = NULL dispatch passed as argument |
| **swsSpotWeldConnectorErrorPlanesNotParallel** | 8 = Planes are not parallel |
| **swsSpotWeldConnectorErrorPlanesTouching** | 9 = Planes touching |
| **swsSpotWeldConnectorErrorPostWeldInvalidPoints** | 12 = Post weld invalid points |
| **swsSpotWeldConnectorErrorSelectAssemblyDocument** | 5 = Select an assembly document |
| **swsSpotWeldConnectorErrorSelectDatumPoints** | 11 = Select datum points for spot weld |
| **swsSpotWeldConnectorErrorSelectFace** | 6 = Select a face |
| **swsSpotWeldConnectorErrorSuccessful** | 0 = Successful |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)