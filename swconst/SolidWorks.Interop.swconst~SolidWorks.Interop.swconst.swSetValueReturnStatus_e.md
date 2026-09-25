<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swSetValueReturnStatus_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swSetValueReturnStatus\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swSetValueReturnStatus\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Return values for attempting to set the value of a parameter.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swSetValueReturnStatus_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swSetValueReturnStatus_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swSetValueReturnStatus_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swSetValueReturnStatus_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swSetValue\_DrivenDimension** | 3 = Cannot be done on a dimension driven by geometry |
| **swSetValue\_Failure** | 1 = Failed for an unknown reason |
| **swSetValue\_FrozenFeatureOwner** | 5 = Owner of the dimension is frozen |
| **swSetValue\_InvalidValue** | 2 = Not a valid value for change parameter |
| **swSetValue\_ModelNotLoaded** | 4 = Model must be loaded in order to set this value |
| **swSetValue\_Successful** | 0 = Successful |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)