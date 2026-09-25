<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFatigueEventEndEditError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsFatigueEventEndEditError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsFatigueEventEndEditError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Fatigue event editing errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsFatigueEventEndEditError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsFatigueEventEndEditError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsFatigueEventEndEditError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsFatigueEventEndEditError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsFatigueEventError\_AssociatedStudyShouldBeStaticNonlinearOrDynamicModalTimeHistory** | 21 = Associated study should be a static, nonlinear, or dynamic modal time history study |
| **swsFatigueEventError\_CannotApplyLoadingRatio** | 12 = Loading ratio is invalid |
| **swsFatigueEventError\_CannotApplyRepeats** | 13 = Cannot apply the specified number of repeats |
| **swsFatigueEventError\_CannotApplyStartTime** | 15 = Cannot apply the specified start time of the fatigue event |
| **swsFatigueEventError\_ImproperEvent** | 2 = Improper fatigue event |
| **swsFatigueEventError\_ImproperNoOfCycles** | 10 = Number of cycles must be greater than 1 and less than 2000000000 |
| **swsFatigueEventError\_ImproperStudy** | 1 = Improper fatigue study |
| **swsFatigueEventError\_ImproperStudyNames** | 3 = Improper associated study names |
| **swsFatigueEventError\_ImproperVarNamesOrVarScalesOrVarSteps** | 18 = Improper variable names, scales, or steps |
| **swsFatigueEventError\_InvalidLoadingtype** | 11 = Loading type must be a number as defined in [swsFatigueLoadingType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFatigueLoadingType_e.html) |
| **swsFatigueEventError\_InvalidRepeats** | 14 = Number of repeats must be greater than 0 and less than 1000000 |
| **swsFatigueEventError\_InvalidStartTime** | 16 = Start time must be greater than 0 |
| **swsFatigueEventError\_LoadHistoryCurveTypeImproper** | 4 = Load history curve type must be a number as defined in [swsFatigueLoadHistoryCurveType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFatigueLoadHistoryCurveType_e.html) |
| **swsFatigueEventError\_NoError** | 0 = Success |
| **swsFatigueEventError\_NoOfPointsShouldBeMoreThan3** | 8 = Load history curve data must have more than 3 points |
| **swsFatigueEventError\_NumberOfStudiesAssociationShouldbeAtleast1** | 19 = Number of associated studies must be greater than 1 |
| **swsFatigueEventError\_NumberOfStudiesAssociationShouldbeAtleast2** | 20 = Number of associated studies must be greater than 2 |
| **swsFatigueEventError\_StudyNamesScalesAndStepsDifferentInNumber** | 17 = Study names, scales, and steps are all different in number |
| **swsFatigueEventError\_XAndYPointsNotSameInNumber** | 7 = X and Y values of the load history curve data are not the same in number |
| **swsFatigueEventError\_XCurveDataImproper** | 5 = X values of load history curve data are improper |
| **swsFatigueEventError\_XPointsShouldBeInIncreasingOrder** | 9 = X coordinate values of the load history curve data must be in order of increasing value |
| **swsFatigueEventError\_YCurveDataImproper** | 6 = Y values of load history curve data are improper |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)