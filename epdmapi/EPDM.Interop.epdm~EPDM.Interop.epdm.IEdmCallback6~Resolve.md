<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6~Resolve.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Resolve Method (IEdmCallback6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCallback6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6.html) : Resolve Method (IEdmCallback6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Handle of the parent window

*ppoItems*
:   Array of [EdmCmdData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html) structures; one structure for each item that needs to be resolved (see **Remarks**)

Resolves multiple errors.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Resolve( _    ByVal lParentWnd As System.Integer, _    ByRef ppoItems() As EdmCmdData _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Resolve(     System.int lParentWnd,    out EdmCmdData[] ppoItems ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Resolve(  &   System.int lParentWnd, &   [Out] array<EdmCmdData>^ ppoItems ) ``` | |

#### Parameters

*lParentWnd*
:   Handle of the parent window

*ppoItems*
:   Array of [EdmCmdData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html) structures; one structure for each item that needs to be resolved (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCallback6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

SOLIDWORKS PDM Professional continues to call this method until all errors are resolved or until this method returns an error code. If you do not properly implement this method to return an error code, you may cause your program to hang.

Contents of each ppoItem EdmCmdData structure:

| Member | Direction | Contents |
| --- | --- | --- |
| mlObjectID1 | Input | ID of the source file that is being copied; 0 if the file is copied from outside the vault |
| mlObjectID2 | Input | ID of the source file's parent folder; 0 if the file is copied from outside the vault |
| mbsStrData1 | Input | Path to the source file |
| mbsStrData2 | Input | Path to the destination file |
| mlLongData1 | Input | Combination of [EdmResolveReason](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmResolveReason.html) bits telling why this method is called |
| mlLongData2 | Output | Combination of [EdmResolveAction](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmResolveAction.html) bits telling SOLIDWORKS PDM Professional how to proceed |

The ppoItems array may contain items that do not need to be resolved. The mlLongData1 struct members for those items are zero.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCallback6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6.html)

[IEdmCallback6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0