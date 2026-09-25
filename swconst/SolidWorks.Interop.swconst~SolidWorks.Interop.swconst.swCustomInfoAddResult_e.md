<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swCustomInfoAddResult_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swCustomInfoAddResult\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swCustomInfoAddResult\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Result codes when adding custom properties.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swCustomInfoAddResult_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swCustomInfoAddResult_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swCustomInfoAddResult_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swCustomInfoAddResult_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swCustomInfoAddResult\_AddedOrChanged** | 0 = Success |
| **swCustomInfoAddResult\_GenericFail** | 1 = Failed to add the custom property |
| **swCustomInfoAddResult\_MismatchAgainstExistingType** | 2 = Existing custom property with the same name has a different type |
| **swCustomInfoAddResult\_MismatchAgainstSpecifiedType** | 3 = Specified value of the custom property does not match the specified type |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)