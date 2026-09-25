<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion5~Rollback.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Rollback Method (IEdmEnumeratorVersion5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmEnumeratorVersion5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion5.html) : Rollback Method (IEdmEnumeratorVersion5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lVersionNo*
:   Version number to which to roll this file back (see **Remarks**)

Obsolete. Superseded by [IEdmEnumeratorVersion6::Rollback2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion6~Rollback2.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Rollback( _    ByVal lVersionNo As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Rollback(     System.int lVersionNo ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Rollback(  &   System.int lVersionNo ) ``` | |

#### Parameters

*lVersionNo*
:   Version number to which to roll this file back (see **Remarks**)

# ![](dotnetimages/collapse.gif)Remarks

This method destroys all versions after the version specified by lVersionNo. There is no undoing of the operation short of restoring a backup of the entire database and file archives.

After this method completes successfully, lVersionNo is the new latest version of the file.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_INVALID\_REVISION\_NUMBER: The specified version number is out of bounds.* E\_EDM\_PERMISSION\_DENIED: The user lacks permission to delete files.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmEnumeratorVersion5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion5.html)

[IEdmEnumeratorVersion5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmEnumeratorVersion5_members.html)

[IEdmVersion5::Rollback Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVersion5~Rollback.html)

[IEdmRevision5::Rollback Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevision5~Rollback.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2