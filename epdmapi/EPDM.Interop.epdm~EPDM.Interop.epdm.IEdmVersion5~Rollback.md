<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion5~Rollback.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Rollback Method (IEdmVersion5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVersion5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion5.html) : Rollback Method (IEdmVersion5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Obsolete. Superseded by [IEdmVersion6::Rollback2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion6~Rollback2.html).

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

This method deletes both the file data and the file data card data when it deletes versions. You cannot undo this rollback, unless you restore a complete backup of the database and the file archives.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_PERMISSION\_DENIED: The user does not have permission to delete files.* E\_EDM\_INVALID\_REVISION\_NUMBER: The version does not exist.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVersion5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion5.html)

[IEdmVersion5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion5_members.html)

[IEdmEnumeratorVersion5::Rollback Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion5~Rollback.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2