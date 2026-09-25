<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistoryUpdate~UpdateVersionComment.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| UpdateVersionComment Method (IEdmHistoryUpdate) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmHistoryUpdate Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistoryUpdate.html) : UpdateVersionComment Method (IEdmHistoryUpdate) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFileID*
:   ID of file for which to update a comment

*lVersionNo*
:   ID of version for which to update a comment; -1 for all versions

*bsNewComment*
:   New version comment

Updates a version comment.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub UpdateVersionComment( _    ByVal lFileID As System.Integer, _    ByVal lVersionNo As System.Integer, _    ByVal bsNewComment As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void UpdateVersionComment(     System.int lFileID,    System.int lVersionNo,    System.string bsNewComment ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void UpdateVersionComment(  &   System.int lFileID, &   System.int lVersionNo, &   System.String^ bsNewComment ) ``` | |

#### Parameters

*lFileID*
:   ID of file for which to update a comment

*lVersionNo*
:   ID of version for which to update a comment; -1 for all versions

*bsNewComment*
:   New version comment

# ![](dotnetimages/collapse.gif)Example

See the [IEdmHistoryUpdate](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistoryUpdate.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, you must call [IEdmHistoryUpdate::CommitUpdates](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistoryUpdate~CommitUpdates.html) to write the change to the database.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmHistoryUpdate Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistoryUpdate.html)

[IEdmHistoryUpdate Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmHistoryUpdate_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2008