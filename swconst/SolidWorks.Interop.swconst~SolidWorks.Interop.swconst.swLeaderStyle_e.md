<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swLeaderStyle_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swLeaderStyle\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swLeaderStyle\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Leader styles.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swLeaderStyle_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swLeaderStyle_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swLeaderStyle_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swLeaderStyle_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swAlwaysAttachToBalloon** | 0x1004 or 4100 = Bitmask; applies only to balloon annotations; specifies that the balloon's **Always Attach to Balloon** leader option is enabled and the leader is always attached to the balloon when quantity is specified, and the balloon's **Break Around** leader option is disabled; if not specified, then the balloon's **Always Attach to Balloon** leader option is disabled, and the balloon's **Break Around** leader option is enabled and the balloon's leader is set to break around quantity; AND with one of the following options:   * swBENT* swSTRAIGHT* swUNDERLINED (parts only)* swSPLINE (drawings only)* swVDA |
| **swAttachLeaderBottom** | 0x400 or 1024 = Bitmask; in part's multiline note, attaches leader to bottom of note; AND with one of the following options:   * swBENT* swSTRAIGHT* swUNDERLINED |
| **swAttachLeaderCenter** | 0x200 or 512 = Bitmask; in a part's multiline note, attaches leader to center of note; AND with one of the following options:   * swBENT* swSTRAIGHT* swUNDERLINED |
| **swAttachLeaderNearest** | 0x800 or 2048 = Bitmask; in a part's multiline note, left leader attaches to the top of note and right leader attaches to the bottom of note; AND with one of the following options:   * swBENT* swSTRAIGHT* swUNDERLINED |
| **swAttachLeaderTop** | 0x100 or 256 = Bitmask; in a part's multiline note, attaches leader to top of note; AND with one of the following options:   * swBENT* swSTRAIGHT* swUNDERLINED |
| **swBENT** | 2 = Creates a bent leader |
| **swNO\_LEADER** | 0 = No leader |
| **swSPLINE** | 4 = Creates a spline leader from a note; for drawings only |
| **swSTRAIGHT** | 1 = Creates a straight leader |
| **swUNDERLINED** | 3 = Creates an underlined leader; for parts only |
| **swVDA** | 8 = Creates an inspection leader |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)