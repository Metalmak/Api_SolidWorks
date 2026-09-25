<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoGen7~GetSerialNumberNames.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetSerialNumberNames Method (IEdmSerNoGen7) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmSerNoGen7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoGen7.html) : GetSerialNumberNames Method (IEdmSerNoGen7) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*ppoRetNames*
:   Array of serial number generator names

Gets the names of all of the serial number generators installed in the vault.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetSerialNumberNames( _    ByRef ppoRetNames() As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetSerialNumberNames(     out System.string[] ppoRetNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetSerialNumberNames(  &   [Out] System.array<String^>^ ppoRetNames ) ``` | |

#### Parameters

*ppoRetNames*
:   Array of serial number generator names

# ![](dotnetimages/collapse.gif)Example

[Set Part Number Using Default Serial Numbers (C#)](Set_Part_Number_Using_Default_Serial_Numbers_Example_CSharp.htm)

[Set Part Number Using Default Serial Numbers (VB.NET)](Set_Part_Number_Using_Default_Serial_Numbers_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmSerNoGen7 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoGen7.html)

[IEdmSerNoGen7 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSerNoGen7_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.4