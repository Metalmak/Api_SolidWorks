<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swOpenDocOptions_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swOpenDocOptions\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swOpenDocOptions\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

How to open documents using ISldWorks::OpenDoc6. Bitmask.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swOpenDocOptions_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swOpenDocOptions_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swOpenDocOptions_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swOpenDocOptions_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swOpenDocOptions\_AdvancedConfig** | 8192 or 0x2000; Open assembly using an advanced configuration |
| **swOpenDocOptions\_AutoMissingConfig** | 32 or 0x20 = Obsolete; do not use  The software automatically uses the last-used configuration of a model when it discovers missing configurations or component references as it silently opens drawings and assemblies. |
| **swOpenDocOptions\_DontLoadHiddenComponents** | 256 or 0x100 = By default, hidden components are loaded when you open an assembly document. Set swOpenDocOptions\_DontLoadHiddenComponents to not load hidden components when opening an assembly document |
| **swOpenDocOptions\_LDR\_EditAssembly** | 2048 or 0x800 = Open in Large Design Review (resolved) mode with edit assembly enabled; use in combination with swOpenDocOptions\_ViewOnly |
| **swOpenDocOptions\_LoadExternalReferencesInMemory** | 512 or 0x200 = Open external references in memory only; this setting is valid only if [swUserPreferenceIntegerValue\_e](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swUserPreferenceIntegerValue_e.html).swLoadExternalReferences is not set to [swLoadExternalReferences\_e](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swLoadExternalReferences_e.html).swLoadExternalReferences\_None  [swUserPreferenceToggle\_e.swExtRefLoadRefDocsInMemory](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swUserPreferenceToggle_e.html) (**System Options > External References > Load documents in memory only**) is ignored when opening documents through the API because IDocumentSpecification::LoadExternalReferencesInMemory and ISldWorks::OpenDoc6 (swOpenDocOptions\_e.swOpenDocOptions\_LoadExternalReferencesInMemory) have sole control of reference loading |
| **swOpenDocOptions\_LoadLightweight** | 128 or 0x80 = Open assembly document as lightweight  NOTE: The default for whether an assembly document is opened lightweight is based on a registry setting accessed via Tools, Options, Assemblies or with the user preference setting swAutoLoadPartsLightweight  To override the default and specify a value with ISldWorks::OpenDoc6, set swOpenDocOptions\_OverrideDefaultLoadLightweight. If set, then you can set swOpenDocOptions\_LoadLightweight to open an assembly document as lightweight |
| **swOpenDocOptions\_LoadModel** | 16 or 0x10 = Load Detached model upon opening document (drawings only) |
| **swOpenDocOptions\_OpenDetailingMode** | 1024 or 0x400 = Open document in detailing mode |
| **swOpenDocOptions\_OverrideDefaultLoadLightweight** | 64 or 0x40 = Override default setting whether to open an assembly document as lightweight |
| **swOpenDocOptions\_RapidDraft** | 8 or 0x8 = Convert document to Detached format (drawings only) |
| **swOpenDocOptions\_ReadOnly** | 2 or 0x2 = Open document read only |
| **swOpenDocOptions\_Silent** | 1 or 0x1 = Open document silently |
| **swOpenDocOptions\_SpeedPak** | 4096 or 0x1000 = Open document using the SpeedPak option |
| **swOpenDocOptions\_ViewOnly** | 4 or 0x4 = Open document in Large Design Review mode only (assemblies only) |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)