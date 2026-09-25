<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swSaveAsOptions_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swSaveAsOptions\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swSaveAsOptions\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Save As options. Bitmask.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swSaveAsOptions_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swSaveAsOptions_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swSaveAsOptions_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swSaveAsOptions_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swSaveAsOptions\_AvoidRebuildOnSave** | 8 or 0x8 |
| **swSaveAsOptions\_Copy** | 2 or 0x2; Save the document as a copy and continue editing |
| **swSaveAsOptions\_CopyAndOpen** | 512 or 0x200; Save the document as a copy and open it |
| **swSaveAsOptions\_DetachedDrawing** | 128 or 0x80; Not a valid option for IPartDoc::SaveToFile2 |
| **swSaveAsOptions\_IgnoreBiography** | 256 or 0x100; Prune a SOLIDWORKS file's revision history to just the current file name |
| **swSaveAsOptions\_IncludeVirtualSubAsmComps** | 1024 or 0x400; Save regular components in virtual subassemblies |
| **swSaveAsOptions\_OverrideSaveEmodel** | 32 or 0x20; Saves eDrawings-related information into a section of the file being saved; specifying this setting overrides the Tools, Options, System Options, General, Save eDrawings data in SOLIDWORKS document setting; not a valid option for IPartDoc::SaveToFile2 |
| **swSaveAsOptions\_SaveEmodelData** | Obsolete. |
| **swSaveAsOptions\_SaveReferenced** | 4 or 0x4; Supports parts, assemblies, and drawings; this setting indicates to save all components (sub-assemblies and parts) in both assemblies and drawings; if a part has an external reference, then this setting indicates to save the external reference |
| **swSaveAsOptions\_Silent** | 1 or 0x1 |
| **swSaveAsOptions\_UpdateInactiveViews** | 16 or 0x10; Not a valid option for IPartDoc::SaveToFile2; this setting is only applicable for a drawing that has one or more sheets; this setting updates the views on inactive sheets |

# ![](dotnetimages/collapse.gif)Remarks

These options only apply to saving to native SOLIDWORKS file formats. For example, to export a SOLIDWORKS file to a VRML file format, use ISldWorks::GetUserPreferenceToggle and ISldWorks::SetUserPreferenceToggle with swExportVrmlAllComponentsInSingleFile.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)