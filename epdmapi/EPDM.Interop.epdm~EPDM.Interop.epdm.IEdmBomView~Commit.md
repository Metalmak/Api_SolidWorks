<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView~Commit.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Commit Method (IEdmBomView) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBomView Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView.html) : Commit Method (IEdmBomView) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsSaveAsBomName*
:   Name of new BOM in which to save the BOM content; empty string to save changes to an existing BOM

*pbsErrorMessage*
:   Error message

*plFocusNodeID*
:   ID of node to which to set focus

Saves the BOM content.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function Commit( _    ByVal bsSaveAsBomName As System.String, _    ByRef pbsErrorMessage As System.String, _    ByRef plFocusNodeID As System.Integer _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int Commit(     System.string bsSaveAsBomName,    out System.string pbsErrorMessage,    out System.int plFocusNodeID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int Commit(  &   System.String^ bsSaveAsBomName, &   [Out] System.String^ pbsErrorMessage, &   [Out] System.int plFocusNodeID ) ``` | |

#### Parameters

*bsSaveAsBomName*
:   Name of new BOM in which to save the BOM content; empty string to save changes to an existing BOM

*pbsErrorMessage*
:   Error message

*plFocusNodeID*
:   ID of node to which to set focus

#### Return Value

[Return codes](ReturnCodes.htm)

# ![](dotnetimages/collapse.gif)Example

[Add Row to Bill of Materials (VB.NET)](Add_Row_to_Bill_of_Materials_Example_VBNET.htm)

[Add Row to Bill of Materials (C#)](Add_Row_to_Bill_of_Materials_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBomView Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView.html)

[IEdmBomView Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBomView_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009