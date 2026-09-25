<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion6~Rollback2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Rollback2 Method (IEdmVersion6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVersion6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion6.html) : Rollback2 Method (IEdmVersion6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsComment*
:   Comment for this rollback

Obsolete. Superseded by [IEdmVersion8::Rollback3](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion8~Rollback3.html).

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
:   Comment for this rollback

# ![](dotnetimages/collapse.gif)Remarks

This method deletes both the file data and the file data card data when it deletes versions. You cannot undo this rollback, unless you restore a complete backup of the database and the file archives.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_PERMISSION\_DENIED: The user does not have permission to delete files.* E\_EDM\_INVALID\_REVISION\_NUMBER: The version does not exist.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVersion6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion6.html)

[IEdmVersion6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion6_members.html)

[IEdmEnumeratorVersion6::Rollback2 Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion6~Rollback2.html)

[IEdmRevision6::Rollback2 Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision6~Rollback2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2015