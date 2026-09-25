<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetFlag.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| EdmGetFlag Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : EdmGetFlag Enumeration |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Options for retrieving files used in calls to [IEdmFile5::GetFileCopy](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile5~GetFileCopy.html), [IEdmEnumeratorVersion5::GetFileCopy](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion5~GetFileCopy.html), [IEdmVersion5::GetFileCopy](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion5~GetFileCopy.html), and [IEdmRevision5::GetFileCopy](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision5~GetFileCopy.html). [Bitmask](Bitmasks.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Public Enum EdmGetFlag     Inherits System.Enum ``` | |

| C# |  |
| --- | --- |
| ``` public enum EdmGetFlag : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class EdmGetFlag : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **EdmGet\_DisableRefresh** | 2 = Do not refresh File Explorer when a file is retrieved |
| **EdmGet\_ForPreview** | 64 = Only retrieve referenced files that are needed by SOLIDWORKS PDM Professional's preview when retrieving the referencing file |
| **EdmGet\_MakeReadOnly** | 1 = Mark the retrieved file as read-only |
| **EdmGet\_Refs** | 4 = Get referenced files |
| **EdmGet\_RefsOnlyMissing** | 8 = Only get referenced files that are not present on the local hard disk; only valid in combination with EdmGet\_Refs |
| **EdmGet\_RefsOverwriteLocked** | 32 = Retrieve checked out referenced files and their references; only valid in combination with EdmGet\_Refs; Warning: Setting this flag means that any previous modifications to checked out files will be lost. |
| **EdmGet\_RefsVerLatest** | 16 = Retrieve the latest versions of referenced files that you have permission to see instead of attached versions that were used when the file was checked in; only valid in combination with EdmGet\_Refs |
| **EdmGet\_Simple** | 0 = Retrieve the file |

# ![](dotnetimages/collapse.gif)See Also

####

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)