<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsLoadsAndRestraintsError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsLoadsAndRestraintsError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsLoadsAndRestraintsError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Loads and restraints errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsLoadsAndRestraintsError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsLoadsAndRestraintsError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsLoadsAndRestraintsError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsLoadsAndRestraintsError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsLoadsAndRestraintsError\_InvalidComponentsCount** | 3 = Number of bodies/components must be greater than one |
| **swsLoadsAndRestraintsError\_InvalidSelection** | 4 |
| **swsLoadsAndRestraintsError\_InvalidSelectionsMixedTogether** | 5 = Non-supported entities selected together |
| **swsLoadsAndRestraintsError\_NotFoundWithGivenName** | 2 = Load or restraint with specified name not found |
| **swsLoadsAndRestraintsErrorNotFoundAtIndex** | 1 = Load or restraint not found at this index |
| **swsLoadsAndRestraintsErrorSuccessful** | 0 = Successful |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)