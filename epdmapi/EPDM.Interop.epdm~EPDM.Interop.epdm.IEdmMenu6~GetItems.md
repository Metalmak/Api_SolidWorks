<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu6~GetItems.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetItems Method (IEdmMenu6) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmMenu6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu6.html) : GetItems Method (IEdmMenu6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lEdmMenuFlags*
:   Types of item you want returned as defined in [EdmMenuFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMenuFlags.html)

*ppoRetItems*
:   Array of [EdmCmdInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdInfo.html) structs of the returned items

Gets the commands that appear on the toolbar.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetItems( _    ByVal lEdmMenuFlags As System.Integer, _    ByRef ppoRetItems() As EdmCmdInfo _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetItems(     System.int lEdmMenuFlags,    out EdmCmdInfo[] ppoRetItems ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetItems(  &   System.int lEdmMenuFlags, &   [Out] array<EdmCmdInfo>^ ppoRetItems ) ``` | |

#### Parameters

*lEdmMenuFlags*
:   Types of item you want returned as defined in [EdmMenuFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmMenuFlags.html)

*ppoRetItems*
:   Array of [EdmCmdInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdInfo.html) structs of the returned items

# ![](dotnetimages/collapse.gif)Example

[Get Menu Command Items (VB.NET)](Get_Menu_Command_Items_Example_VBNET.htm)

[Get Menu Command Items (C#)](Get_Menu_Command_Items_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Calling [IEdmMenu5::GetToolbarItemIDs](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5~GetToolbarItemIDs.html), [IEdmMenu5::GetButtonImages](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5~GetButtonImages.html), or [IEdmMenu5::GetString](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5~GetString.html) also gets the commands that should appear on the toolbar.

[Return code](ReturnCodes.htm) S\_OK indicates that the method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmMenu6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu6.html)

[IEdmMenu6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009