<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsUserPreferenceToggle_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsUserPreferenceToggle\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsUserPreferenceToggle\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

User preference toggle values

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsUserPreferenceToggle_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsUserPreferenceToggle_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsUserPreferenceToggle_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsUserPreferenceToggle_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsAverageStressesAtMidnodes** | 17 = Get or set whether to average stresses at mid-nodes; corresponds to **Simulation > Options > Default Options > Results > Average stresses at mid-nodes (high-quality solid mesh only)** |
| **swsColorChartColorNoOfChartColorFlip** | 13 = Get or set whether to flip the chart colors; corresponds to **Simulation > Options > Default Options > Plot > Color Chart > Color options > Flip** |
| **swsColorChartColorSpecifyColorForvonMisesPlot** | 14 = Get or set whether to specify color for values above yield for vonMises plot; corresponds to **Simulation > Options > Default Options > Plot > Color Chart > Color options > Specify color for values above yield for vonMises plot** |
| **swsColorChartDetails** | 11 = Get or set whether to display plot details; corresponds to **Simulation > Options > Default Options > Plot > Color Chart > Display plot details** |
| **swsColorChartDisplay** | 10 = Get or set whether to display plot details; corresponds to **Simulation > Options > Default Options > Plot > Color Chart > Display color charts** |
| **swsColorChartNumberFormatUseDifferentNumberFormat** | 12 = Get or set whether to use a different number format for small numbers; corresponds to **Simulation > Options > Default Options > Plot > Color Chart > Number format > Scientific > Use different number format for small numbers (0.001 < |x| < 1000)** |
| **swsEMailAuthentication** | 16 = Get or set whether my server requires authentication; corresponds to **Simulation > Options > System Options > Email Notification Settings > My server requires authentication** |
| **swsLoadAllStudies\_e** | 15 = Get or set whether to load all Simulation studies when opening a model; corresponds to **Simulation > Options > System Options > General > Load all Simulation studies when opening a model. (requires more time to open a model)** |
| **swsPlotAnnotationShowMaxValue** | 5 = Get or set whether to show the maximum value annotation in plots; corresponds to **Simulation > Options > Default Options > Plot > Annotation and range > Show maximum value annotation** |
| **swsPlotAnnotationShowMinValue** | 4 = Get or set whether to show the minimum value annotation in plots; corresponds to **Simulation > Options > Default Options > Plot > Annotation and range > Show minimum value annotation** |
| **swsPlotAnnotationShowRangeBasedOnShowCompOnly** | 6 = Get or set whether to show range based on shown components only in plots; corresponds to **Simulation > Options > Default Options > Plot > Annotation and range > Show range based on shown components only** |
| **swsPlotDeformedShapeOptionSuperImposeModelOnDeformedShape** | 9 = Get or set whether to superimpose model on deformed shape in plots; corresponds to **Simulation > Options > Default Options > Plot > Deformed shape options > Show rsults on deformed shape > Superimpose model on deformed shape** |
| **swsPlotShowExcludedBodies** | 7 = Get or set whether to show excluded bodies in plots; corresponds to **Simulation > Options > Default Options > Plot > Settings options > Show excluded bodies** |
| **swsPlotShowHiddenBodies** | 8 = Get or set whether to show hidden bodies in plots; corresponds to **Simulation > Options > Default Options > Plot > Settings options > Show hidden bodies** |
| **swsResultFolderKeepTempDataBase** | 1 = Get or set whether to keep temporary database files in results folder; corresponds to **Simulation > Options > Default Options > Results > Results folder > Keep temporary database files** |
| **swsResultFolderUnderSubFolder** | 0 = Get or set whether to set results folder under a SOLIDWORKS document folder sub folder; corresponds to **Simulation > Options > Default Options > Results > Results folder > SOLIDWORKS document folder > Under sub folder** |
| **swsShowReportOnPublish** | 3 = Get or set whether to show the report when it's published; corresponds to **Simulation > Options > Default Options > Report > Report publish options > Show report on publish** |
| **swsTrendTrackerBackUpModelsRestoreIteration** | 2 = Get or set whether to back up models for Restore to Iteration; corresponds to **Simulation > Options > Default Options > Results > Trend Tracker > Backup models for Restore to Iteration** |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)