<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault6~GetCardID.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetCardID Method (IEdmVault6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault6.html) : GetCardID Method (IEdmVault6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eType*
:   Type of card to get as defined in [EdmCardType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardType.html)

*bsName*
:   Name of the card to get

*lFolderID*
:   ID of the folder in which the card is stored; 0 for search cards and template

Gets the ID of a card of the specified type, with the specified name, and in the specified folder.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetCardID( _    ByVal eType As EdmCardType, _    ByVal bsName As System.String, _    Optional ByVal lFolderID As System.Integer _ ) As System.Integer ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetCardID(     EdmCardType eType,    System.string bsName,    System.int lFolderID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetCardID(  &   EdmCardType eType, &   System.String^ bsName, &   System.int lFolderID ) ``` | |

#### Parameters

*eType*
:   Type of card to get as defined in [EdmCardType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardType.html)

*bsName*
:   Name of the card to get

*lFolderID*
:   ID of the folder in which the card is stored; 0 for search cards and template

#### Return Value

Card ID; 0 if not found

# ![](dotnetimages/collapse.gif)Remarks

After calling this method, you can use the returned ID in calls to [IEdmVault5::GetObject](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~GetObject.html) or [IEdmVault6::CreateCardViewEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault6~CreateCardViewEx.html).

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* S\_FALSE: The specified card was not found.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault6.html)

[IEdmVault6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.0