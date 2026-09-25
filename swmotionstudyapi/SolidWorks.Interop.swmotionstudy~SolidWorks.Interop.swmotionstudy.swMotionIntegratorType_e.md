<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.swMotionIntegratorType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| swMotionIntegratorType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html) : swMotionIntegratorType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Integration methods for solving numerically stiff systems.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swMotionIntegratorType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swMotionIntegratorType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swMotionIntegratorType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swMotionIntegratorType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swMotionIntegrator\_GSTIFF** | 1 = Default integration method for fast and accurate computation of displacements; variable order and step size; coefficients are calculated assuming a constant step size |
| **swMotionIntegrator\_SI2\_GSTIFF** | 3 = Stabilized Index-2 integration method that provides better error control over the velocity and acceleration terms in equations of motion; provided motion is sufficiently smooth, velocity and acceleration results are more accurate than those computed with GSTIFF or WSTIFF; significantly slower |
| **swMotionIntegrator\_WSTIFF** | 2 = Variable order and step size integration method; coefficients are calculated as a function of the step size; handles sudden step size changes as a result of discontinuities or abrupt events without error or loss of accuracy |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html)