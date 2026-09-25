<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~GetErrorName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetErrorName Method (IEdmVault11) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11.html) : GetErrorName Method (IEdmVault11) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lHRESULT*
:   Error code for which to get the internal name

Gets an internal error code name for the specified error code.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetErrorName( _    ByVal lHRESULT As System.Integer _ ) As System.String ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetErrorName(     System.int lHRESULT ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetErrorName(  &   System.int lHRESULT ) ``` | |

#### Parameters

*lHRESULT*
:   Error code for which to get the internal name

#### Return Value

Internal error code name

# ![](dotnetimages/collapse.gif)Example

[Get and Set Item References (C#)](Get_and_Set_Item_References_Example_CSharp.htm)

[Get and Set Item References (VB.NET)](Get_and_Set_Item_References_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method returns the internal error code name for an HRESULT error code. For example, if lHRESULT is 0x80040204, this method returns "E\_EDM\_NOT\_LOGGED\_IN".

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault11 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11.html)

[IEdmVault11 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11_members.html)

[IEdmVault11::GetErrorMessage Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault11~GetErrorMessage.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2010