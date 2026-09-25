<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr8~ShowUserPopup.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| ShowUserPopup Method (IEdmUserMgr8) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserMgr8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr8.html) : ShowUserPopup Method (IEdmUserMgr8) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*hParent*
:   Handle of the parent window

*poTrackRect*
:   [EdmRect](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRect.html) structure; bounding rectangle of the area in the window that will trigger the mouse hover event

*oUserID*
:   ID, login name, or full name of the user for which to display information in the popup window (see **Remarks**)

Displays a popup window with information about the specified user when the mouse hovers over the specified area of the specified window.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub ShowUserPopup( _    ByVal hParent As System.Integer, _    ByRef poTrackRect As EdmRect, _    ByVal oUserID As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void ShowUserPopup(     System.int hParent,    ref EdmRect poTrackRect,    System.object oUserID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ShowUserPopup(  &   System.int hParent, &   EdmRect% poTrackRect, &   System.Object^ oUserID ) ``` | |

#### Parameters

*hParent*
:   Handle of the parent window

*poTrackRect*
:   [EdmRect](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRect.html) structure; bounding rectangle of the area in the window that will trigger the mouse hover event

*oUserID*
:   ID, login name, or full name of the user for which to display information in the popup window (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmUserMgr8](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr8.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

In the SOLIDWORKS PDM Professional user interface, whenever the mouse hovers over a user name, a popup window displays information about the user. The popup window displays until the mouse moves off the area containing the user name. Call this method to display a popup window when the mouse hovers over a user name in a Windows form.

If oUserID contains a full name that is not unique, the user to display is randomly selected by the system.

[IEdmUser10::SetUserDataEx](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUser10~SetUserDataEx.html) describes how to update the information displayed in the popup window.

Call [IEdmUserMgr8::CreateUserPicture](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr8~CreateUserPicture.html) if you want to display the picture of a user in a Windows form.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* E\_INVALIDARG: One or more of the arguments are invalid.* E\_EDM\_NOT\_LOGGED\_IN: You must log in to the vault before calling this method.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserMgr8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr8.html)

[IEdmUserMgr8 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr8_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013