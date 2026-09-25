<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsDropTestSetUpError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsDropTestSetUpError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsDropTestSetUpError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Setup errors for drop test studies

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsDropTestSetUpError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsDropTestSetUpError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsDropTestSetUpError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsDropTestSetUpError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsDropTestSetUpError\_AvailableOnlyForDropTestStudy** | 1 = Not available for this study type |
| **swsDropTestSetUpError\_GravityEntityIsNULL** | 3 = Gravity entity is NULL |
| **swsDropTestSetUpError\_GravityEntityShouldBeEdgeFaceOrPlane** | 4 = Gravity entity should be an edge, face, or plane |
| **swsDropTestSetUpError\_NoError** | 0 = No error |
| **swsDropTestSetUpError\_SetUpAlreadyAdded** | 2 = Setup already exists |
| **swsDropTestSetUpError\_SetupNotExists** | 6 = Setup does not exist |
| **swsDropTestSetUpError\_ShouldBeStraightEdgeOrPlaneFace** | 5 = Gravity entity should be straight edge or planar face |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)