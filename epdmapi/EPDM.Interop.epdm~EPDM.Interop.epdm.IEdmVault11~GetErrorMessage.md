<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~GetErrorMessage.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetErrorMessage Method (IEdmVault11) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11.html) : GetErrorMessage Method (IEdmVault11) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lHRESULT*
:   Error code for which to get a description

Gets a description for the specified error code.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetErrorMessage( _    ByVal lHRESULT As System.Integer _ ) As System.String ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetErrorMessage(     System.int lHRESULT ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetErrorMessage(  &   System.int lHRESULT ) ``` | |

#### Parameters

*lHRESULT*
:   Error code for which to get a description

#### Return Value

Description of the error code

# ![](dotnetimages/collapse.gif)Example

[Add Items (C#)](Add_Items_Example_CSharp.htm)

[Add Items (VB.NET)](Add_Items_Example_VBNET.htm)

[Add Users (C#)](Add_Users_Example_CSharp.htm)

[Add Users (VB.NET)](Add_Users_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method returns a readable error message for HRESULT error codes. For example, if lHRESULT is 0x80040204, then this method returns "You have not logged in to the file vault."

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11.html)

[IEdmVault11 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11_members.html)

[IEdmVault11::GetErrorName Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~GetErrorName.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010