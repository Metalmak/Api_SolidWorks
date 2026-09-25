<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swLinkDimensionError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swLinkDimensionError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swLinkDimensionError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Link dimension errors.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swLinkDimensionError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swLinkDimensionError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swLinkDimensionError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swLinkDimensionError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swLinkDimensionError\_AlreadyLinked** | 4 = Dimension already linked elsewhere |
| **swLinkDimensionError\_CannotLink** | 8 = The selected dimensions cannot be linked; combination of failures swLinkDimensionError\_LinkAcrossDocs to swLinkDimensionError\_DrivenByEquation |
| **swLinkDimensionError\_DrivenByEquation** | 7 = Dimension's driven by an equation |
| **swLinkDimensionError\_EmptyString** | 11 = Empty string passed as link text |
| **swLinkDimensionError\_ErrorUknown** | 0 = Unknown error occurred |
| **swLinkDimensionError\_IncompatibleDimTypes** | 3 = Cannot link incompatible dimension types |
| **swLinkDimensionError\_IncompatibleValues** | 6 = Incompatible range of values make these dimensions not linkable |
| **swLinkDimensionError\_InvalidString** | 12 = Invalid string passed as link text; cannot contain the at sign (@) character |
| **swLinkDimensionError\_LinkAcrossDocs** | 2 = Values to be linked must belong to the same model |
| **swLinkDimensionError\_NoError** | 1 = No error; success |
| **swLinkDimensionError\_ReadOnlyOrDriven** | 5 = Dimension is a read-only, driven, or a reference dimension that cannot be linked |
| **swLinkDimensionError\_UnableToCreateSharedParam** | 9 = Shared parameter could not be created |
| **swLinkDimensionError\_UnlinkFailure** | 10 = Dimension was not already linked |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)