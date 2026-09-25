<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swCheckInterferenceOption_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swCheckInterferenceOption\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swCheckInterferenceOption\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Check interference options. Bitmask.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swCheckInterferenceOption_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swCheckInterferenceOption_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swCheckInterferenceOption_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swCheckInterferenceOption_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swBodyInterference\_IncludeCoincidentFaces** | 2 or 0x2; Abutment (i.e., faces touching each other) type of clash |
| **swBodyInterference\_OptionDefault** | 1 or 0x1; If this option specified, then swBodyInterference\_IncludeCoincidentFaces and swBodyInterference\_ReturnInterferingObject are set to false |
| **swBodyInterference\_ReturnInterferingObject** | 4 or 0x4; Return face and body arrays |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)