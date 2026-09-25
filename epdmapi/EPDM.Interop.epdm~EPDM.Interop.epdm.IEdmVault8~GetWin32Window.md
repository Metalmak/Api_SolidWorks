<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault8~GetWin32Window.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetWin32Window Method (IEdmVault8) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault8.html) : GetWin32Window Method (IEdmVault8) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lHwnd*
:   Window handle to convert

Converts the specified window handle to an Win32Window interface that can be used in the .NET Framework.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetWin32Window( _    ByVal lHwnd As System.Integer _ ) As System.Object ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetWin32Window(     System.int lHwnd ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetWin32Window(  &   System.int lHwnd ) ``` | |

#### Parameters

*lHwnd*
:   Window handle to convert

#### Return Value

IWin32Window interface

# ![](dotnetimages/collapse.gif)Example

[Creating Add-ins (VB.NET)](DotNetAddIns.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault8.html)

[IEdmVault8 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault8_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.4