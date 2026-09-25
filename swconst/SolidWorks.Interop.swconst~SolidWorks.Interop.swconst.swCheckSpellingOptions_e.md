<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swCheckSpellingOptions_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swCheckSpellingOptions\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swCheckSpellingOptions\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Spell check options. Bitmask.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swCheckSpellingOptions_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swCheckSpellingOptions_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swCheckSpellingOptions_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swCheckSpellingOptions_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swSpellingIgnoreCapitalizedWords** | 8 or 0x8; Capitalized words are not checked |
| **swSpellingIgnoreInternetAndFiles** | 16 or 0x10; Words containing a web address are not checked |
| **swSpellingIgnoreMixedCase** | 2 or 0x2; Words that are mixed-case (upper case and lowercase, e.g., eDrawings) are not checked |
| **swSpellingIgnoreUpperCase** | 1 or 0x1; Words that are all uppercase are not checked |
| **swSpellingIgnoreWordsWithNumbers** | 4 or 0x4; Words containing both letters and numbers are not checked |
| **swSpellingLeaveEngineRunning** | 32 or 0x20; Do not stop Microsoft Word, which is the spell-check engine, after checking the first and any subsequent annotations if you have a significant number of annotations to spell check; however, on the last use of IAnnotation::CheckSpelling, you must disable this flag so that Microsoft Word is shut down after that call |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)