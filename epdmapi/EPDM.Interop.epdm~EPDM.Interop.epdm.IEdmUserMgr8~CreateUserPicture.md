<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr8~CreateUserPicture.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| CreateUserPicture Method (IEdmUserMgr8) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmUserMgr8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr8.html) : CreateUserPicture Method (IEdmUserMgr8) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*hParent*
:   Handle of parent window on which the picture should be drawn

*poDestRect*
:   [EdmRect](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRect.html) structure; bounding rectangle in which the picture should be drawn (see **Remarks**)

*oUserID*
:   ID or login name of the user for which to create a picture

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) to receive progress information if the picture needs to be downloaded from an archive server

*lEdmUserPictureFlags*
:   Combination of [EdmUserPictureFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserPictureFlag.html) bits

Creates a picture of the user to display in a form.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function CreateUserPicture( _    ByVal hParent As System.Integer, _    ByRef poDestRect As EdmRect, _    ByVal oUserID As System.Object, _    Optional ByVal poCallback As EdmCallback, _    Optional ByVal lEdmUserPictureFlags As System.Integer _ ) As IEdmImage ``` | |

| C# |  |
| --- | --- |
| ``` IEdmImage CreateUserPicture(     System.int hParent,    ref EdmRect poDestRect,    System.object oUserID,    EdmCallback poCallback,    System.int lEdmUserPictureFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmImage^ CreateUserPicture(  &   System.int hParent, &   EdmRect% poDestRect, &   System.Object^ oUserID, &   EdmCallback^ poCallback, &   System.int lEdmUserPictureFlags ) ``` | |

#### Parameters

*hParent*
:   Handle of parent window on which the picture should be drawn

*poDestRect*
:   [EdmRect](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmRect.html) structure; bounding rectangle in which the picture should be drawn (see **Remarks**)

*oUserID*
:   ID or login name of the user for which to create a picture

*poCallback*
:   Optional pointer to a class that implements [IEdmCallback](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCallback.html) to receive progress information if the picture needs to be downloaded from an archive server

*lEdmUserPictureFlags*
:   Combination of [EdmUserPictureFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmUserPictureFlag.html) bits

#### Return Value

[IEdmImage](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmImage.html)

# ![](dotnetimages/collapse.gif)Example

See the [IEdmUserMgr8](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr8.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Call [IEdmUserMgr8::ShowUserPopup](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr8~ShowUserPopup.html) to display a popup window with user information.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmUserMgr8 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr8.html)

[IEdmUserMgr8 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmUserMgr8_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013