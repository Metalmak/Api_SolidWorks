<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsResultPlotErrorCode_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsResultPlotErrorCode\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsResultPlotErrorCode\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Result plot error codes

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsResultPlotErrorCode_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsResultPlotErrorCode_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsResultPlotErrorCode_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsResultPlotErrorCode_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsResultPlot\_CosworksViewNotPresent** | 16 = Cosmos view is not present |
| **swsResultPlot\_EquivalentStressNotApplicable** | 15 = Equivalent stress plot is not applicable |
| **swsResultPlot\_FailedPlotCreation** | 2 = Plot not created |
| **swsResultPlot\_ImproperResultsEquation** | 13 = Invalid results equation |
| **swsResultPlot\_InvalidComponentType** | 6 = Invalid result component type |
| **swsResultPlot\_InvalidExternalResultsFile** | 17 |
| **swsResultPlot\_InvalidInputArgInCombiWithTensorVectorFlag** | 4 = Tensor plot cannot be rendered when "Render Shell in 3D" or "Show plot on selected entities" is selected |
| **swsResultPlot\_InvalidIsoValueRange** | 18 |
| **swsResultPlot\_InvalidMeshAppliedToStudy** | 9 = Mesh not compatible with study type |
| **swsResultPlot\_InvalidResultType** | 5 = Invalid result type |
| **swsResultPlot\_InvalidSelectedEntities** | 3 = Invalid selected entities |
| **swsResultPlot\_InvalidSmoothingCycleRange** | 19 |
| **swsResultPlot\_InvalidStudy** | 1 = Study is missing important internal components |
| **swsResultPlot\_InvalidStudyType** | 12 = Step numbers not compatible with study type |
| **swsResultPlot\_InvalidUnitType** | 7 = Invalid unit type |
| **swsResultPlot\_IsAvailableOnlyForElements** | 8 = Plot is valid only for elements |
| **swsResultPlot\_IsAvailableOnlyForNodes** | 11 = Plot is valid only for nodes |
| **swsResultPlot\_MeshInformationNotFound** | 20 |
| **swsResultPlot\_NoError** | 0 = No error |
| **swsResultPlot\_PlotDoesNotExist** | 14 = Result plot does not exist |
| **swsResultPlot\_TryingToSetInvalidProperty** | 10 = Invalid property |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)