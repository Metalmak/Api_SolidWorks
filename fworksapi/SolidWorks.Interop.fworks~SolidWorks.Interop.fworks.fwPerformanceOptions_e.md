<!-- source: fworksapi/SolidWorks.Interop.fworks~SolidWorks.Interop.fworks.fwPerformanceOptions_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| FeatureWorks API Help | Send Feedback |
| fwPerformanceOptions\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.fworks Namespace](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks_namespace.html) : fwPerformanceOptions\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Performance options.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum fwPerformanceOptions_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As fwPerformanceOptions_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum fwPerformanceOptions_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class fwPerformanceOptions_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **fwDoNotPerformBodyCheck** | 0x0001 = When you do not specify this option, the software periodically checks the body during feature recognition; if this option is specified, then the software does not check the body for any errors (resulting in faster performance) |
| **fwDoNotPerformIntrusionCheck** | 0x0002 = When you specify this option, the software does not check for features that intrude upon one another during automatic feature recognition |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.fworks Namespace](SolidWorks.Interop.fworks~SolidWorks.Interop.fworks_namespace.html)