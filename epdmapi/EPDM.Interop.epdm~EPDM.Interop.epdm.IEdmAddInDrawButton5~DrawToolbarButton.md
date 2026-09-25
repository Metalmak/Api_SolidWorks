<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInDrawButton5~DrawToolbarButton.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| DrawToolbarButton Method (IEdmAddInDrawButton5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmAddInDrawButton5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInDrawButton5.html) : DrawToolbarButton Method (IEdmAddInDrawButton5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lCmdID*
:   Command ID passed to [IEdmCmdMgr5::AddCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddCmd.html) during add-in registration

*hDC*
:   Handle of the device context to draw on

*poDestRect*
:   [EdmRect](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRect.html) structure; rectangle within which to draw

*eState*
:   State of the button image to draw as defined in [EdmButtonState](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmButtonState.html)

*plRetBackgroundColor*
:   RGB value of a transparent color

Dynamically draws an add-in toolbar button.

**NOTE:** This method does not work in Windows Vista and later Windows operating systems.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub DrawToolbarButton( _    ByVal lCmdID As System.Integer, _    ByVal hDC As System.Integer, _    ByRef poDestRect As EdmRect, _    ByVal eState As EdmButtonState, _    ByRef plRetBackgroundColor As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void DrawToolbarButton(     System.int lCmdID,    System.int hDC,    ref EdmRect poDestRect,    EdmButtonState eState,    out System.int plRetBackgroundColor ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void DrawToolbarButton(  &   System.int lCmdID, &   System.int hDC, &   EdmRect% poDestRect, &   EdmButtonState eState, &   [Out] System.int plRetBackgroundColor ) ``` | |

#### Parameters

*lCmdID*
:   Command ID passed to [IEdmCmdMgr5::AddCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddCmd.html) during add-in registration

*hDC*
:   Handle of the device context to draw on

*poDestRect*
:   [EdmRect](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRect.html) structure; rectangle within which to draw

*eState*
:   State of the button image to draw as defined in [EdmButtonState](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmButtonState.html)

*plRetBackgroundColor*
:   RGB value of a transparent color

# ![](dotnetimages/collapse.gif)Example

#### Visual Basic sample code showing how to dynamically draw a toolbar button

1. Add the toolbar button command in the [IEdmAddIn5::GetAddInInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~GetAddInInfo.html) implementation:

> poCmdMgr.AddCmd 1000, "First command", EdmMenu\_HasToolbarButton Or EdmMenu\_OwnerDrawToolbarButton, "This is the first command", "First command", -1, -1

2. At the top of your class implementation, add declarations of the Win32 GDI functions that you want to use (read more about this in the Visual Basic online help):

> Private Declare Sub LineTo Lib "Gdi32" (ByVal hDC As Long, ByVal X As Long, ByVal Y As Long)
>
> Private Declare Sub MoveToEx Lib "Gdi32" (ByVal hDC As Long, ByVal X As Long, ByVal Y As Long, ByVal OldPnt As Long)
>
> Private Declare Sub Arc Lib "Gdi32" (ByVal hDC As Long, \_
>                                      ByVal x1 As Long, ByVal y1 As Long, \_
>                                      ByVal x2 As Long, ByVal y2 As Long, \_
>                                      ByVal xstart As Long, ByVal ystart As Long, \_
>                                      ByVal xend As Long, ByVal yend As Long)

3. Implement IEdmAddInDrawButton5::DrawToolbarButton (called by SOLIDWORKS PDM Professional):

> Private Sub IEdmAddInDrawButton5\_DrawToolbarButton(ByVal lCmdID As Long, ByVal hDC As Long, poDestRect As EdmRect, ByVal eState As EdmButtonState, plRetBackgroundColor As Long)
> On Error GoTo ErrHand
>
> If eState = BState\_Cold Then
>   'Draw a cross using the default pen
>   MoveToEx hDC, poDestRect.mlLeft, poDestRect.mlTop, 0
>   LineTo hDC, poDestRect.mlRight, poDestRect.mlBottom
>   MoveToEx hDC, poDestRect.mlLeft, poDestRect.mlBottom, 0
>   LineTo hDC, poDestRect.mlRight, poDestRect.mlTop
> Else
>   'Draw a circle using the default pen
>   Arc hDC, poDestRect.mlLeft, poDestRect.mlTop, poDestRect.mlRight, poDestRect.mlBottom, \_
>   poDestRect.mlLeft + (poDestRect.mlRight - poDestRect.mlLeft) / 2, poDestRect.mlTop, \_
>   poDestRect.mlLeft + (poDestRect.mlRight - poDestRect.mlLeft) / 2, poDestRect.mlTop
> End If
>
> Exit Sub
> ErrHand:
> Dim errnum As String
> errnum = Err.Number
> MsgBox "Error drawing toolbar button!" + vbLf + Err.Description + vbLf + errnum
> End Sub

# ![](dotnetimages/collapse.gif)Remarks

See the [IEdmAddInDrawButton5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInDrawButton5.html) topic for more information.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmAddInDrawButton5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInDrawButton5.html)

[IEdmAddInDrawButton5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInDrawButton5_members.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.2 of SOLIDWORKS PDM Professional