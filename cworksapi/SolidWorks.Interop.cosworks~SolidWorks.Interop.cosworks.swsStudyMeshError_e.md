<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsStudyMeshError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsStudyMeshError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsStudyMeshError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Mesh study errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsStudyMeshError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsStudyMeshError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsStudyMeshError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsStudyMeshError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsStudyErrorElementSizeTooBig** | 4 = Element size is too large; specify a smaller element size |
| **swsStudyErrorElementSizeTooSmall** | 3 = Element size is too small; specify a larger element size to run successfully |
| **swsStudyErrorNoSolidBody** | 2 = No solid body to process |
| **swsStudyErrorNoValidShells** | 1 = No valid shells defined |
| **swsStudyErrorSpecifyElementSizeScaleFactor** | 6 = Specify a number between 0.1 and 10 for element size scale factor |
| **swsStudyErrorSpecifyPositiveValue** | 5 = Specify a positive value |
| **swsStudyErrorSpecifyToleranceScaleFactor** | 7 = Specify a number between 0.01 and 100 for tolerance scale factor |
| **swsStudyErrorSuccessful** | 0 = Successful |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)