<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swPMContainer_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swPMContainer\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swPMContainer\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Docking states of PropertyManager page.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swPMContainer_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swPMContainer_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swPMContainer_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swPMContainer_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swPMFloating** | 3 = True floating state where PropertyManager page lives inside new docking pane; a single floating window owns all PropertyManager pages of all open documents |
| **swPMInTabsWithFM** | 0 = Old-style PropertyManager page embedded in tabs at top |
| **swPMPinnedAboveFM** | 1 = Quasi floating state where PropertyManager page automatically displays, resizes itself in the lower-left corner of model frame window, and covers the FeatureManager design tree; one window for each open document |
| **swPMPinnedLowerRight** | 4 = Quasi floating state where PropertyManager page automatically displays, resizes itself in the lower-right corner of the model frame window, covers the graphic area, and has full height;  one window for each open document |
| **swPMPinnedNextToFM** | 2 = Quasi floating state where PropertyManager page automatically displays, resizes itself to the right of the FeatureManager design tree, covers the graphics area, and has full height.; one window for each open document |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)