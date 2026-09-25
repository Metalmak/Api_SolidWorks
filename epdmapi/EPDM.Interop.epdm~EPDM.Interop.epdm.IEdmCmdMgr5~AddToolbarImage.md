<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddToolbarImage.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AddToolbarImage Method (IEdmCmdMgr5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCmdMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5.html) : AddToolbarImage Method (IEdmCmdMgr5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lHandleOrResourceID*
:   Resource ID if bIsHandle = false; handle to a bitmap (bIsIcon = false) or icon (bIsIcon = true) if bIsHandle = true

*lButtonCount*
:   Number of buttons in the bitmap or icon

*eState*
:   State of the toolbar button (see **Remarks**)

*bIsIcon*
:   True if the image is an icon; false if it is a bitmap (see **Remarks**)

*bIsHandle*
:   True if lHandleOrResourceID is a handle, false if it is a resource ID

*lBackgroundColorRGB*
:   RGB value of the background color (see **Remarks**)

*lImageID*
:   ID of the image (see **Remarks**)

Registers an image with a toolbar button.

**NOTE:** This method does not work in Windows Vista and later Windows operating systems.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AddToolbarImage( _    ByVal lHandleOrResourceID As System.Integer, _    ByVal lButtonCount As System.Integer, _    ByVal eState As EdmButtonState, _    Optional ByVal bIsIcon As System.Boolean, _    Optional ByVal bIsHandle As System.Boolean, _    Optional ByVal lBackgroundColorRGB As System.Integer, _    Optional ByVal lImageID As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AddToolbarImage(     System.int lHandleOrResourceID,    System.int lButtonCount,    EdmButtonState eState,    System.bool bIsIcon,    System.bool bIsHandle,    System.int lBackgroundColorRGB,    System.int lImageID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddToolbarImage(  &   System.int lHandleOrResourceID, &   System.int lButtonCount, &   EdmButtonState eState, &   System.bool bIsIcon, &   System.bool bIsHandle, &   System.int lBackgroundColorRGB, &   System.int lImageID ) ``` | |

#### Parameters

*lHandleOrResourceID*
:   Resource ID if bIsHandle = false; handle to a bitmap (bIsIcon = false) or icon (bIsIcon = true) if bIsHandle = true

*lButtonCount*
:   Number of buttons in the bitmap or icon

*eState*
:   State of the toolbar button (see **Remarks**)

*bIsIcon*
:   True if the image is an icon; false if it is a bitmap (see **Remarks**)

*bIsHandle*
:   True if lHandleOrResourceID is a handle, false if it is a resource ID

*lBackgroundColorRGB*
:   RGB value of the background color (see **Remarks**)

*lImageID*
:   ID of the image (see **Remarks**)

# ![](dotnetimages/collapse.gif)Example

For a more complete description of how to use this method, see [Creating a menu command](vbmenuitem.htm).

The following snippet creates a toolbar button and adds a command in the File Explorer Tools menu. The button uses one icon (resource ID=101) for the cold (standard) state and another one (resource ID=102) for the hot (focus) state. Both icon files must be added using Visual Basic's resource editor before running this snippet:

Private Sub IEdmAddIn5\_GetAddInInfo(poInfo As EdmAddInInfo, ByVal poVault As IEdmVault5, ByVal poCmdMgr As IEdmCmdMgr5)

> ...
> poCmdMgr.AddToolbarImage 101, 1, BState\_Cold, True, False, 12632256, 1
> poCmdMgr.AddToolbarImage 102, 1, BState\_Hot, True, False, 12632256, 1
> poCmdMgr.AddCmd 1, "My Command", EdmMenu\_NeverInContextMenu Or EdmMenu\_HasToolbarButton, "String to show in the statusbar", "Tooltip on my command", 0, 1

End Sub

# ![](dotnetimages/collapse.gif)Remarks

Call this method from your add-in's implementation of [IEdmAddIn5::GetAddInInfo](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddIn5~GetAddInInfo.html) to create a toolbar button.

Images can be either bitmaps (\*.BMP) or icons (\*.ICO). A bitmap contains one or more buttons of the same size. An icon contains only one button.

Unlike icons, bitmaps do not contain transparent regions. In order to get transparency in bitmaps, specify in lBackgroundColorRGB the RGB color of the bitmap that should be replaced by the background color.

When you add "hot" buttons (eState = [EdmButtonState](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmButtonState.html).BState\_Hot), they must be assigned the same image ID as the corresponding "cold" buttons (eState = EdmButtonState.BState\_Cold). Additionally, if the images contain several toolbar buttons, the buttons must be ordered the same way in both images.

Toolbar buttons in File Explorer can have several different sizes depending on the operating system version, Internet Explorer version, and user preferences. To make the image compatible, use this method to add several versions of an image using the same image ID but with different image sizes. SOLIDWORKS PDM Professional chooses the image that best matches the system settings. If the image doesn't exactly match the button size, PDM either resizes it (if the button is smaller than the image) or centers it in the button (if the button is bigger than the image).

After calling this method to create a toolbar button, call [IEdmCmdMgr5::AddCmd](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5~AddCmd.html) setting lToolbarImageID to this method's lImageID.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCmdMgr5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5.html)

[IEdmCmdMgr5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCmdMgr5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2