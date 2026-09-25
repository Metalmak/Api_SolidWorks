<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision6~Rollback2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Rollback2 Method (IEdmRevision6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRevision6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision6.html) : Rollback2 Method (IEdmRevision6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsComment*
:   Comment for this revision

Obsolete. Superseded by [IEdmRevision7::Rollback3](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision7~Rollback3.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Rollback2( _    ByVal bsComment As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Rollback2(     System.string bsComment ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Rollback2(  &   System.String^ bsComment ) ``` | |

#### Parameters

*bsComment*
:   Comment for this revision

# ![](dotnetimages/collapse.gif)Remarks

This method destroys all versions after this revision number. To undo this rollback operation, you need to restore a backup of the entire database and file archives.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_PERMISSION\_DENIED: The user lacks permission to delete files.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRevision6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision6.html)

[IEdmRevision6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision6_members.html)

[IEdmEnumeratorVersion6::Rollback2 Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion6~Rollback2.html)

[IEdmVersion6::Rollback2 Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion6~Rollback2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2015