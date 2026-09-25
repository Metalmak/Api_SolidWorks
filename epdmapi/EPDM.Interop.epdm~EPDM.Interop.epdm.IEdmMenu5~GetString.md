<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5~GetString.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetString Method (IEdmMenu5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmMenu5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5.html) : GetString Method (IEdmMenu5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lItemID*
:   ID of menu item for which to get a string

*eType*
:   Type of string to get as defined in [EdmMenuStrType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMenuStrType.html)

Gets a string for a menu item in this menu.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetString( _    ByVal lItemID As System.Integer, _    ByVal eType As EdmMenuStrType _ ) As System.String ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetString(     System.int lItemID,    EdmMenuStrType eType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetString(  &   System.int lItemID, &   EdmMenuStrType eType ) ``` | |

#### Parameters

*lItemID*
:   ID of menu item for which to get a string

*eType*
:   Type of string to get as defined in [EdmMenuStrType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMenuStrType.html)

#### Return Value

String (see **Remarks**)

# ![](dotnetimages/collapse.gif)Remarks

C++ programmers must free the returned string with SysFreeString.

[Return code](ReturnCodes.htm) S\_OK indicates that the method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmMenu5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5.html)

[IEdmMenu5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5_members.html)

[IEdmMenu6::GetItems Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu6~GetItems.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.2 of SOLIDWORKS PDM Professional