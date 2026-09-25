<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile12~GetLocalVersionNo2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetLocalVersionNo2 Method (IEdmFile12) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFile12 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile12.html) : GetLocalVersionNo2 Method (IEdmFile12) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPathOrFolderID*
:   ID of a folder, full file path, or folder path of the local copy of this file (see **Remarks**)

*pbLocalOverwrittenVersionObsolete*
:   True if the file in the user's local cache is obsolete, false if it is valid (see **Remarks**)

Gets the version number of the local copy of this file.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetLocalVersionNo2( _    ByRef poPathOrFolderID As System.Object, _    ByRef pbLocalOverwrittenVersionObsolete As System.Boolean _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetLocalVersionNo2(     ref System.object poPathOrFolderID,    out System.bool pbLocalOverwrittenVersionObsolete ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetLocalVersionNo2(  &   System.Object^% poPathOrFolderID, &   [Out] System.bool pbLocalOverwrittenVersionObsolete ) ``` | |

#### Parameters

*poPathOrFolderID*
:   ID of a folder, full file path, or folder path of the local copy of this file (see **Remarks**)

*pbLocalOverwrittenVersionObsolete*
:   True if the file in the user's local cache is obsolete, false if it is valid (see **Remarks**)

#### Return Value

Version number; -1 if the local copy does not match any version in the archive

# ![](dotnetimages/collapse.gif)Remarks

If poPathOrFolderID is a folder path, it must be terminated by a backslash ('\').

pbLocalOverwrittenVersionObsolete gets whether a file in a user's local cache is obsolete because the file was overwritten by another user who checked out the file, modified the file, and checked in the file.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFile12 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile12.html)

[IEdmFile12 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFile12_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2017