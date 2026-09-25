<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr3~VerUpgrade_BumpRevisions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| VerUpgrade\_BumpRevisions Method (IEdmRevisionMgr3) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRevisionMgr3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr3.html) : VerUpgrade\_BumpRevisions Method (IEdmRevisionMgr3) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poFiles*
:   Array of [EdmSelItem](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem.html) structures; one structure for each file on which to bump the revision number (see **Remarks**)

Moves all revisions set on the second-to-latest version to the latest version.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub VerUpgrade_BumpRevisions( _    ByVal poFiles() As EdmSelItem _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void VerUpgrade_BumpRevisions(     EdmSelItem[] poFiles ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void VerUpgrade_BumpRevisions(  &   array<EdmSelItem>^ poFiles ) ``` | |

#### Parameters

*poFiles*
:   Array of [EdmSelItem](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSelItem.html) structures; one structure for each file on which to bump the revision number (see **Remarks**)

# ![](dotnetimages/collapse.gif)Remarks

You need to be logged in as a user that has permission to update revision numbers ([EdmSysRightFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmSysRightFlags.html).EdmSysRight\_ModifyRevisionNumbers) in order to use this method. The reason you need this high level of permission is that this method overrides other permission settings on the file and changes the content of file history.

poFiles contains the array of files on which to bump revision numbers. Files lacking revisions on the second-to-latest version are ignored.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRevisionMgr3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr3.html)

[IEdmRevisionMgr3 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr3_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009