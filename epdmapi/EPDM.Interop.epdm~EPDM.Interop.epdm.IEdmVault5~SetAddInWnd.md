<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5~SetAddInWnd.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetAddInWnd Method (IEdmVault5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html) : SetAddInWnd Method (IEdmVault5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lAddInWnd*
:   Add-in window handle

*lParentWnd*
:   File Explorer window handle; [EdmCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd.html)::mlParentWnd passed to [IEdmAddIn5::OnCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html)

Obsolete. See [Keeping Add-in Windows in the Foreground](KeepWindowInfront.htm).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetAddInWnd( _    ByVal lAddInWnd As System.Integer, _    ByVal lParentWnd As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetAddInWnd(     System.int lAddInWnd,    System.int lParentWnd ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetAddInWnd(  &   System.int lAddInWnd, &   System.int lParentWnd ) ``` | |

#### Parameters

*lAddInWnd*
:   Add-in window handle

*lParentWnd*
:   File Explorer window handle; [EdmCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmd.html)::mlParentWnd passed to [IEdmAddIn5::OnCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~OnCmd.html)

# ![](dotnetimages/collapse.gif)Remarks

This method ensures that windows created from add-ins written in Visual Basic 6 do not appear behind the application window. Since VBA is no longer supported, this method is obsolete and should not be used.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVault5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5.html)

[IEdmVault5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVault5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2