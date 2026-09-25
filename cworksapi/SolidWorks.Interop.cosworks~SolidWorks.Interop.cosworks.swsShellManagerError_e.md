<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsShellManagerError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsShellManagerError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsShellManagerError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Shell creation errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsShellManagerError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsShellManagerError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsShellManagerError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsShellManagerError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsShellManagerErrorCannotApplyShellForMesh** | 2 = Shell cannot be applied for this mesh type |
| **swsShellManagerErrorCannotApplyShellForStudy** | 1 = Shell cannot be applied for this study type |
| **swsShellManagerErrorEmptyArray** | 3 = Empty array; no faces selected |
| **swsShellManagerErrorFaceAlreadyDefinedAsShell** | 6 = A face is already defined as a shell |
| **swsShellManagerErrorFaceAlreadyExists** | 7 = At least on face is specified more than once |
| **swsShellManagerErrorInvalidArray** | 4 = Invalid array |
| **swsShellManagerErrorSelectFacesOnly** | 5 = Select faces only |
| **swsShellManagerErrorSuccessful** | 0 = Successful |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)