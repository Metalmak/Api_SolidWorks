<!-- source: swmotionstudyapi/SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy.swMotionStudyType_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Motion Study API Help | Send comments on this topic. |
| swMotionStudyType\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html) : swMotionStudyType\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Motion study types. Bitmask.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swMotionStudyType_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swMotionStudyType_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swMotionStudyType_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swMotionStudyType_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swMotionStudyTypeAssembly** | 1 or 0x1 = Animation; D-cubed solver is used to do presentation animation only; no simulation is performed, so no results or plots are available; gravity, contact, springs, and forces cannot be used; mass and inertia values have no effect on the animation |
| **swMotionStudyTypeCosmosMotion** | 4 or 0x4 = Motion Analysis; ADAMS (MSC.Software) solver is used to return accurate results; you must load the SOLIDWORKS Motion add-in with a SOLIDWORKS premium license to use this option |
| **swMotionStudyTypeLegacyCosmosMotion** | 8 or 0x8 = Legacy COSMOSMotion; in SOLIDWORKS 2007 and earlier, motion analysis was provided through the COSMOSMotion add-in; this option is available if either the COSMOSMotion add-in is loaded or you open an older model that was created using that add-in; models with legacy COSMOSMotion data can be opened but not edited |
| **swMotionStudyTypeNewCosmosMotion** | 16 or 0x10 |
| **swMotionStudyTypePhysicalSimulation** | 2 or 0x2 = Basic Motion; NVIDIA phys-x solver is used to perform fast and approximate dynamic analysis; quickly returns results that look realistic at the cost of accuracy |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swmotionstudy Namespace](SolidWorks.Interop.swmotionstudy~SolidWorks.Interop.swmotionstudy_namespace.html)