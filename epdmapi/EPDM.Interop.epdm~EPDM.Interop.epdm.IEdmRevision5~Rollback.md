<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision5~Rollback.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Rollback Method (IEdmRevision5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRevision5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision5.html) : Rollback Method (IEdmRevision5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Obsolete. Superseded by [IEdmRevision6::Rollback2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision6~Rollback2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Rollback() ``` | |

| C# |  |
| --- | --- |
| ``` void Rollback() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Rollback(); ``` | |

# ![](dotnetimages/collapse.gif)Remarks

This method destroys all versions after this revision number. To undo this rollback operation, you need to restore a backup of the entire database and file archives.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_PERMISSION\_DENIED: The user lacks permission to delete files.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRevision5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision5.html)

[IEdmRevision5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2