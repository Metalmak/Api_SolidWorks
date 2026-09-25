<!-- source: swconst/SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swFileSaveError_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Enumerations | Send comments on this topic. |
| swFileSaveError\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html) : swFileSaveError\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

File save errors. Bitmask.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swFileSaveError_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swFileSaveError_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swFileSaveError_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swFileSaveError_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swFileLockError** | 16 or 0x10 |
| **swFileNameContainsAtSign** | 8 or 0x8 = File name cannot contain the at symbol (@) |
| **swFileNameEmpty** | 4 or 0x4 = File name cannot be empty |
| **swFileSaveAsBadEDrawingsVersion** | 1024 or 0x400 |
| **swFileSaveAsDoNotOverwrite** | 128 or 0x80 = Do not overwrite an existing file |
| **swFileSaveAsInvalidFileExtension** | 256 or 0x100 = File name extension does not match the SOLIDWORKS document type |
| **swFileSaveAsNameExceedsMaxPathLength** | 2048 or 0x800 = File name cannot exceed 255 characters |
| **swFileSaveAsNoSelection** | 512 or 0x200 = Save the selected bodies in a part document. Valid option for IPartDoc::SaveToFile2; however, not a valid option for IModelDocExtension::SaveAs |
| **swFileSaveAsNotSupported** | 4096 or 0x1000 = Save As operation:   * is not supported* was executed is such a way that the resulting file might not be complete, possibly because SOLIDWORKS is hidden; if the error persists after setting SOLIDWORKS to visible and re-attempting the Save As operation, contact SOLIDWORKS API support. |
| **swFileSaveFormatNotAvailable** | 32 or 0x20 = Save As file type is not valid |
| **swFileSaveRequiresSavingReferences** | 8192 or 0x2000 = Saving an assembly with renamed components requires saving the references |
| **swFileSaveWithRebuildError** | Obsolete = See [swFileSaveWarning\_e](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst.swFileSaveWarning_e.html) |
| **swGenericSaveError** | 1 or 0x1 |
| **swReadOnlySaveError** | 2 or 0x2 |

# ![](dotnetimages/collapse.gif)Remarks

Not all of these return codes are fatal errors. The return code is a bitmask of different conditions that can occur during the operation, some of which are fatal and some are informational or warnings.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.swconst Namespace](SolidWorks.Interop.swconst~SolidWorks.Interop.swconst_namespace.html)