<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr~Commit.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Commit Method (IEdmRevisionMgr) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRevisionMgr Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr.html) : Commit Method (IEdmRevisionMgr) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsComment*
:   Comment to show in the file history of revision increments

*ppoErrors*
:   Array of [EdmRevError](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevError.html) structures; one structure for each error that occurred during processing

Commits all of the changes made in this batch object.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Commit( _    ByVal bsComment As System.String, _    ByRef ppoErrors() As EdmRevError _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Commit(     System.string bsComment,    out EdmRevError[] ppoErrors ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Commit(  &   System.String^ bsComment, &   [Out] array<EdmRevError>^ ppoErrors ) ``` | |

#### Parameters

*bsComment*
:   Comment to show in the file history of revision increments

*ppoErrors*
:   Array of [EdmRevError](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRevError.html) structures; one structure for each error that occurred during processing

# ![](dotnetimages/collapse.gif)Example

[Set Initial Revision (VB.NET)](Set_Initial_Revision_Example_VBNET.htm)

[Set Initial Revision (C#)](Set_Initial_Revision_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRevisionMgr Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr.html)

[IEdmRevisionMgr Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRevisionMgr_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2007