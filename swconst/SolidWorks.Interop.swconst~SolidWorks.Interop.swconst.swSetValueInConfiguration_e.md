<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swSetValueInConfiguration_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swSetValueInConfiguration\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swSetValueInConfiguration\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Values for indicating in which configurations the value should be set.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swSetValueInConfiguration_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swSetValueInConfiguration_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swSetValueInConfiguration_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swSetValueInConfiguration_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swSetValue\_InAllConfigurations** | 2 = Set the value in all configurations |
| **swSetValue\_InSpecificConfigurations** | 3 = Set the value in the specific configuration |
| **swSetValue\_InThisConfiguration** | 1 = Set the value in the current configuration only |
| **swSetValue\_NoConfiguration** | -1 = Ignore configurations in drawing sketches |
| **swSetValue\_UseCurrentSetting** | 0 = Use whatever setting this parameter currently has |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)