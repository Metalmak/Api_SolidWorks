<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion7~Rollback3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Rollback3 Method (IEdmEnumeratorVersion7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnumeratorVersion7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion7.html) : Rollback3 Method (IEdmEnumeratorVersion7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lVersionNo*
:   Version number to which to roll this file back (see **Remarks**)

*bsComment*
:   Comment for the rollback

*vbRedirectParentRefs*
:   True to roll back the file with parent references, false to roll back the file without parent references

Rolls this file back to the specified version.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Rollback3( _    ByVal lVersionNo As System.Integer, _    ByVal bsComment As System.String, _    ByVal vbRedirectParentRefs As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Rollback3(     System.int lVersionNo,    System.string bsComment,    System.bool vbRedirectParentRefs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Rollback3(  &   System.int lVersionNo, &   System.String^ bsComment, &   System.bool vbRedirectParentRefs ) ``` | |

#### Parameters

*lVersionNo*
:   Version number to which to roll this file back (see **Remarks**)

*bsComment*
:   Comment for the rollback

*vbRedirectParentRefs*
:   True to roll back the file with parent references, false to roll back the file without parent references

# ![](dotnetimages/collapse.gif)Remarks

This method destroys all versions after the version specified by lVersionNo. There is no undoing of the operation short of restoring a backup of the entire database and file archives.

After this method completes successfully, lVersionNo is the new latest version of the file.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_INVALID\_REVISION\_NUMBER: The specified version number is out of bounds.* E\_EDM\_PERMISSION\_DENIED: The user lacks permission to delete files.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorVersion7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion7.html)

[IEdmEnumeratorVersion7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion7_members.html)

[IEdmRevision7::Rollback3 Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision7~Rollback3.html)

[IEdmVersion8::Rollback3 Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion8~Rollback3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2017