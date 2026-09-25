<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem~SetProperty.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetProperty Method (IEdmRefItem) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmRefItem Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem.html) : SetProperty Method (IEdmRefItem) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*eProperty*
:   Type of property to update as defined in [EdmRefItemProperty](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefItemProperty.html)

*oValue*
:   New property value

Updates the specified property of this item.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetProperty( _    ByVal eProperty As EdmRefItemProperty, _    ByVal oValue As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetProperty(     EdmRefItemProperty eProperty,    System.object oValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetProperty(  &   EdmRefItemProperty eProperty, &   System.Object^ oValue ) ``` | |

#### Parameters

*eProperty*
:   Type of property to update as defined in [EdmRefItemProperty](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRefItemProperty.html)

*oValue*
:   New property value

# ![](dotnetimages/collapse.gif)Example

[Access Check-in Flags in Check out Dialog (C#)](Access_Check-in_Flags_in_Check_in_Dialog_Example_CSharp.htm)

[Access Check-in Flags in Check out Dialog (VB.NET)](Access_Check-in_Flags_in_Check_in_Dialog_Example_VBNET.htm)

[Prevent Admin from Checking In File (C#)](Prevent_Admin_from_Checking_In_File_Example_CSharp.htm)

[Prevent Admin from Checking In File (VB.NET)](Prevent_Admin_from_Checking_In_File_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_INVALIDARG: The eProperty argument contains a property that cannot be updated in this container, or oValue does not match the type specified in eProperty.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmRefItem Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem.html)

[IEdmRefItem Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmRefItem_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.4