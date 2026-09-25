<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsPVResultCombinationError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsPVResultCombinationError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsPVResultCombinationError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Errors when combining results of Pressure Vessel Design studies

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsPVResultCombinationError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsPVResultCombinationError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsPVResultCombinationError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsPVResultCombinationError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsPVResultCombinationError\_AtleastTwoItemsNeeded** | 2 = You need to specify at least two studies and multiplication factors |
| **swsPVResultCombinationError\_CombineAnalysisNotDone** | 7 = The analysis was not done |
| **swsPVResultCombinationError\_CombineIncompatibleConfiguration** | 10 = Incompatible configurations |
| **swsPVResultCombinationError\_CombineIncompatibleConnectors** | 15 = Incompatible connectors |
| **swsPVResultCombinationError\_CombineIncompatibleContact** | 14 = Incompatible contacts |
| **swsPVResultCombinationError\_CombineIncompatibleMesh** | 9 = Incompatible meshes |
| **swsPVResultCombinationError\_CombineIncompatiblePlanarType** | 16 = Incompatible planar types |
| **swsPVResultCombinationError\_CombineIncompatibleRestraints** | 11 = Incompatible restraints |
| **swsPVResultCombinationError\_CombineIncompatibleResults** | 8 = Incompatible results |
| **swsPVResultCombinationError\_CombineIncompatibleShellsMaterials** | 13 = Incompatible shell materials |
| **swsPVResultCombinationError\_CombineIncompatibleSolidsMaterials** | 12 = Incompatible solid materials |
| **swsPVResultCombinationError\_InvalidFactors** | 5 = One or more multiplication factors are invalid |
| **swsPVResultCombinationError\_InvalidStudy** | 6 = One or more studies are invalid |
| **swsPVResultCombinationError\_ItemsNotSameInNumber** | 4 = Number of elements in the multiplication factors and study names arrays are not the same |
| **swsPVResultCombinationError\_NoError** | 0 = Successful |
| **swsPVResultCombinationError\_NotAvailable** | 1 = Result combination is not available for this study |
| **swsPVResultCombinationError\_StudyNamesNotProper** | 3 = Study names are not valid |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)