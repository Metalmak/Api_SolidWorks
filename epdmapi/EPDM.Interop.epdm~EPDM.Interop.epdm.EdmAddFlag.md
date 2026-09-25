<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmAddFlag.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmAddFlag Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmAddFlag Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Options for adding a file to a folder to the vault, copying a file or folder within the vault, or copying/moving a tree of files and folders. [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmAddFlag     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmAddFlag : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmAddFlag : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmAdd\_DeleteSource** | 64 = Delete the source file once it has been added to the vault |
| **EdmAdd\_DoNotCopy** | 512 = Do not physically copy the file during the add operations because the file has already been copied |
| **EdmAdd\_DontAddCorrupt** | 2 = Refuse to add corrupt files; [IEdmFolder5::AddFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFolder5~AddFile.html) returns the error code [E\_EDM\_INVALID\_FILE](ReturnCodes.htm) |
| **EdmAdd\_ForceGenerateSerialNumbers** | 128 = Force regeneration of serial numbers when values already exist; if this flag is not set, SOLIDWORKS PDM Professional will only generate values that are missing in the file |
| **EdmAdd\_GetInterface** | 256 = Return the file interface; only works with [IEdmBatchAdd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchAdd.html) |
| **EdmAdd\_KeepExistingSerialNumbers** | 4 = Do not replace existing serial numbers with new ones; SOLIDWORKS PDM Professional still creates serial numbers for empty fields; if this flag is not set, SOLIDWORKS PDM Professional writes over existing serial numbers with new ones |
| **EdmAdd\_Refresh** | 1 = Make all file listings in File Explorer and Open/Save As dialog boxes refresh so that the new file is displayed |
| **EdmAdd\_Simple** | 0 = Add the file |
| **EdmAdd\_UniqueVarClearDuplicate** | 16 = Clear duplicated unique constrained variables instead of failing |
| **EdmAdd\_UniqueVarDelayCheck** | 32 = Delay the unique variable check until the next check-in |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)