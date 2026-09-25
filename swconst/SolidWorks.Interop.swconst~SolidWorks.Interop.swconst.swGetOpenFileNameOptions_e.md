<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swGetOpenFileNameOptions_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swGetOpenFileNameOptions\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swGetOpenFileNameOptions\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Options for opening a file returned by ISldWorks::GetOpenFileName2. Bitmask.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swGetOpenFileNameOptions_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swGetOpenFileNameOptions_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swGetOpenFileNameOptions_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swGetOpenFileNameOptions_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swGetOpenFileNameOptions\_AdvancedConfig** | 0x2000; "<Advanced>" selected in configuration dropdown |
| **swGetOpenFileNameOptions\_AutoMissingConfig** | 0x20; Reserved for internal use |
| **swGetOpenFileNameOptions\_DontLoadHiddenComponents** | 0x100; Does not load hidden components (assemblies only) |
| **swGetOpenFileNameOptions\_LDR\_EditAssembly** | 0x800; Reserved for internal use |
| **swGetOpenFileNameOptions\_LoadExternalReferencesInMemory** | 0x200; Reserved for internal use |
| **swGetOpenFileNameOptions\_LoadLightweight** | 0x80; Opens the document in lightweight mode |
| **swGetOpenFileNameOptions\_LoadModel** | 0x10; Reserved for internal use |
| **swGetOpenFileNameOptions\_OpenDetailingMode** | 0x400; Opens the document in detailing mode without part and assembly data (drawings only) |
| **swGetOpenFileNameOptions\_OverrideDefaultLoadLightweight** | 0x40; Reserved for internal use |
| **swGetOpenFileNameOptions\_RapidDraft** | 0x8; Reserved for internal use |
| **swGetOpenFileNameOptions\_ReadOnly** | 0x2; Opens the document read only |
| **swGetOpenFileNameOptions\_SelectedSheets** | 0x8000; "Selected" is checked in Select Sheet to load dialog |
| **swGetOpenFileNameOptions\_Silent** | 0x1; Reserved for internal use |
| **swGetOpenFileNameOptions\_SpeedPak** | 0x1000; Uses Speedpak (assemblies only) |
| **swGetOpenFileNameOptions\_UseLargeAssemblySettings** | 0x4000; Uses large assembly settings (assemblies only) |
| **swGetOpenFileNameOptions\_ViewOnly** | 0x4; Opens the document view only; returned if "None" is selected in Select Sheet to load dialog |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)