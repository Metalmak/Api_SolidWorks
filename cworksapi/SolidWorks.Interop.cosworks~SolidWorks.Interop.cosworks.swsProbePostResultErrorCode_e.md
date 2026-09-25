<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsProbePostResultErrorCode_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsProbePostResultErrorCode\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsProbePostResultErrorCode\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Results probe error codes

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsProbePostResultErrorCode_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsProbePostResultErrorCode_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsProbePostResultErrorCode_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsProbePostResultErrorCode_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsProbePostResultError\_ActiveStudyIsNotRun** | 6 = Active Simulation study must be analyzed before results can be probed |
| **swsProbePostResultError\_InitializationFailure** | 11 = Unable to probe results; re-run the study and try again |
| **swsProbePostResultError\_InvalidOrEmptyInputArray** | 5 = Invalid or empty node/element list |
| **swsProbePostResultError\_MeshDataLoadFailure** | 7 = Unable to load mesh data; remesh the study and try again |
| **swsProbePostResultError\_NoActiveStudy** | 2 = No active study found; activate a Simulation study and try again |
| **swsProbePostResultError\_NoActiveView** | 1 = No active view is available |
| **swsProbePostResultError\_NoAssociatedStudyFoundForFatigueAnalysis** | 12 = No associated study for fatigue analysis was found |
| **swsProbePostResultError\_NoResultOrMeshPlotIsActivated** | 13 = No mesh or result plot was found; re-run the study and try again |
| **swsProbePostResultError\_NotAllNodeElemsAreAnnotated** | 14 = Not all of the specified nodes or elements are annotated |
| **swsProbePostResultError\_ProbingNotSupportedOnDeformationPlot** | 9 = Probing is not supported for deformation result plot |
| **swsProbePostResultError\_ProbingNotSupportedOnSectionPlotExplodedAfterClip** | 10 = Probing is not supported for exploded after clip section result plot |
| **swsProbePostResultError\_ProbingNotSupportedOnShellForSectionPlot** | 8 = Probing is not supported for shell or section result plot |
| **swsProbePostResultError\_ResultPlotActivationFailure** | 3 = Failed to activate the selected result plot |
| **swsProbePostResultError\_Success** | 0 |
| **swsProbePostResultError\_UsedBeforeCallingBeginProbing** | 4 = Cannot make the current results probe edit; call [ICWResultsProbeManager::BeginProbing](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResultsProbeManager~BeginProbing.html) before making results probe edits |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)