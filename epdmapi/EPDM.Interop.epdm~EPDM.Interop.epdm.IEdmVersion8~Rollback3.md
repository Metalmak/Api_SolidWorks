<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion8~Rollback3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Rollback3 Method (IEdmVersion8) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVersion8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion8.html) : Rollback3 Method (IEdmVersion8) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsComment*
:   Comment for this rollback

*vbRedirectParentRefs*
:   True to roll back the file with its parent references, false to roll back the file without its parent references

Discards all versions of the file after this version.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Rollback3( _    ByVal bsComment As System.String, _    ByVal vbRedirectParentRefs As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Rollback3(     System.string bsComment,    System.bool vbRedirectParentRefs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Rollback3(  &   System.String^ bsComment, &   System.bool vbRedirectParentRefs ) ``` | |

#### Parameters

*bsComment*
:   Comment for this rollback

*vbRedirectParentRefs*
:   True to roll back the file with its parent references, false to roll back the file without its parent references

# ![](dotnetimages/collapse.gif)Remarks

This method deletes both the file data and the file data card data when it deletes versions. You cannot undo this rollback, unless you restore a complete backup of the database and the file archives.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_EDM\_PERMISSION\_DENIED: The user does not have permission to delete files.* E\_EDM\_INVALID\_REVISION\_NUMBER: The version does not exist.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVersion8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion8.html)

[IEdmVersion8 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion8_members.html)

[IEdmRevision7::Rollback3 Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision7~Rollback3.html)

[IEdmEnumeratorVersion7::Rollback3 Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion7~Rollback3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2017