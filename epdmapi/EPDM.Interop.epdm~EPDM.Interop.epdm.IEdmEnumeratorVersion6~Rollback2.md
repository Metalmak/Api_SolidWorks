<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion6~Rollback2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Rollback2 Method (IEdmEnumeratorVersion6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnumeratorVersion6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion6.html) : Rollback2 Method (IEdmEnumeratorVersion6) |

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

Obsolete. Superseded by [IEdmEnumeratorVersion7::Rollback3](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion7~Rollback3.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Rollback2( _    ByVal lVersionNo As System.Integer, _    ByVal bsComment As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Rollback2(     System.int lVersionNo,    System.string bsComment ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Rollback2(  &   System.int lVersionNo, &   System.String^ bsComment ) ``` | |

#### Parameters

*lVersionNo*
:   Version number to which to roll this file back (see **Remarks**)

*bsComment*
:   Comment for the rollback

# ![](dotnetimages/collapse.gif)Remarks

This method destroys all versions after the version specified by lVersionNo. There is no undoing of the operation short of restoring a backup of the entire database and file archives.

After this method completes successfully, lVersionNo is the new latest version of the file.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_INVALID\_REVISION\_NUMBER: The specified version number is out of bounds.* E\_EDM\_PERMISSION\_DENIED: The user lacks permission to delete files.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorVersion6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion6.html)

[IEdmEnumeratorVersion6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion6_members.html)

[IEdmVersion6::Rollback2 Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion6~Rollback2.html)

[IEdmRevision6::Rollback2 Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision6~Rollback2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2015