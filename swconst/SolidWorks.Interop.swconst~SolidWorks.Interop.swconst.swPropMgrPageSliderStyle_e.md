<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swPropMgrPageSliderStyle_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swPropMgrPageSliderStyle\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swPropMgrPageSliderStyle\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

PropertyManager page slider styles. Bitmask.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swPropMgrPageSliderStyle_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swPropMgrPageSliderStyle_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swPropMgrPageSliderStyle_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swPropMgrPageSliderStyle_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swPropMgrPageSliderStyle\_AutoTicks** | 2 or 0x2; If set, then tick marks are created based on swPropMgrPageSliderStyle\_BottomLeftTicks and swPropMgrPageSliderStyle\_TopRightTicks |
| **swPropMgrPageSliderStyle\_BottomLeftTicks** | 4 or 0x4; If set, then tick marks appear at the bottom (horizontal) or left (vertical) of the slider |
| **swPropMgrPageSliderStyle\_NotifyWhileTracking** | 16 or 0x10; If set, then your application is notified when the user is dragging the slider, each time the value changes; if not set, then your application is not notified when the user is dragging the slider, only when the user is done dragging the slider; setting this bit allows your application to react immediately to changes, but it does generate many more callbacks, so it is less efficient |
| **swPropMgrPageSliderStyle\_TopRightTicks** | 8 or 0x8; If set, then tick marks appear at the top (horizontal) or right (vertical) of the slider |
| **swPropMgrPageSliderStyle\_Vertical** | 1 or 0x1; If set, then the slider is oriented vertically; if not set, then the slider is oriented horizontally |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)