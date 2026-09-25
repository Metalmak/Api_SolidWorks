<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsShellEndEditError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsShellEndEditError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsShellEndEditError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Shell editing errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsShellEndEditError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsShellEndEditError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsShellEndEditError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsShellEndEditError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsShellEndEditErrorFaceAlreadyDefinedAsShell** | 6 = This face is already defined as shell |
| **swsShellEndEditErrorFaceAlreadyExists** | 5 = At least one face is specified more than once |
| **swsShellEndEditErrorFormulation** | 2 = Specify either 0 or 1 for formulation |
| **swsShellEndEditErrorNoEntitySelected** | 7 = Shell cannot be edited. No entity selected |
| **swsShellEndEditErrorNotEntityAtIndex** | 3 = No entity at index passed for removal |
| **swsShellEndEditErrorOffsetOption** | 9 = Specify shell offset option |
| **swsShellEndEditErrorOffsetValue** | 10 = Specify shell offset value |
| **swsShellEndEditErrorSelectFace** | 4 = Specify face for entity |
| **swsShellEndEditErrorShellThickness** | 1 = Specify a number between 1e-007 and 1e+006 for shell thickness |
| **swsShellEndEditErrorSuccessful** | 0 = Successful |
| **swsShellEndEditErrorUnit** | 8 = Specify 0 to 5 for unit |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)