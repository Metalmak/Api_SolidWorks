<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItemContainer~GetItems.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetItems Method (IEdmRefItemContainer) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRefItemContainer Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItemContainer.html) : GetItems Method (IEdmRefItemContainer) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eType*
:   Type of items to get as defined in [EdmRefItemType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefItemType.html)

*ppoRetItems*
:   Array of [IEdmRefItem](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem.html)s; one interface for each reference item

Gets items from this container.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetItems( _    ByVal eType As EdmRefItemType, _    ByRef ppoRetItems() As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetItems(     EdmRefItemType eType,    out System.object[] ppoRetItems ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetItems(  &   EdmRefItemType eType, &   [Out] System.array<Object^>^ ppoRetItems ) ``` | |

#### Parameters

*eType*
:   Type of items to get as defined in [EdmRefItemType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefItemType.html)

*ppoRetItems*
:   Array of [IEdmRefItem](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem.html)s; one interface for each reference item

# ![](dotnetimages/collapse.gif)Example

[Access Check-in Flags in Check out Dialog (C#)](Access_Check-in_Flags_in_Check_in_Dialog_Example_CSharp.htm)

[Access Check-in Flags in Check out Dialog (VB.NET)](Access_Check-in_Flags_in_Check_in_Dialog_Example_VBNET.htm)

[Prevent Admin from Checking In File (C#)](Prevent_Admin_from_Checking_In_File_Example_CSharp.htm)

[Prevent Admin from Checking In File (VB.NET)](Prevent_Admin_from_Checking_In_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRefItemContainer Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItemContainer.html)

[IEdmRefItemContainer Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItemContainer_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.4