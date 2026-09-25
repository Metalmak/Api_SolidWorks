<!-- source: fworksapi/SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.fwFeatureCreationOptions_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| FeatureWorks API Help | Send Feedback |
| fwFeatureCreationOptions\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.fworks Namespace](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks_namespace.html) : fwFeatureCreationOptions\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Feature creation options. Bitmask.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum fwFeatureCreationOptions_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As fwFeatureCreationOptions_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum fwFeatureCreationOptions_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class fwFeatureCreationOptions_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **fwAddConstraintsToSketch** | 0x1 = When you specify this option, the software adds a Fix relation to each entity in a sketch, fully defining the sketch; if this option is not specified, then the sketch entities remain underdefined |
| **fwAllowFailFeatureCreation** | 0x2 = When you specify this option, the software allows the creation of a feature even if the feature has a rebuild error |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.fworks Namespace](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks_namespace.html)