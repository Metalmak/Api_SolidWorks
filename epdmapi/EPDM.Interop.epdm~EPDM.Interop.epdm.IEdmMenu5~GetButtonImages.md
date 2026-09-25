<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5~GetButtonImages.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetButtonImages Method (IEdmMenu5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmMenu5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5.html) : GetButtonImages Method (IEdmMenu5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*hDestImageList*
:   Handle of the image list (HIMAGELIST) to which to add images; the images are appended at the end of the list

*eState*
:   State of buttons to get as defined in [EdmButtonState](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmButtonState.html)

*poItemIDArray*
:   Array of menu command IDs for which to get images

Gets the toolbar-button images of a range of commands.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetButtonImages( _    ByVal hDestImageList As System.Integer, _    ByVal eState As EdmButtonState, _    ByVal poItemIDArray() As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetButtonImages(     System.int hDestImageList,    EdmButtonState eState,    System.int[] poItemIDArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetButtonImages(  &   System.int hDestImageList, &   EdmButtonState eState, &   System.array<int>^ poItemIDArray ) ``` | |

#### Parameters

*hDestImageList*
:   Handle of the image list (HIMAGELIST) to which to add images; the images are appended at the end of the list

*eState*
:   State of buttons to get as defined in [EdmButtonState](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmButtonState.html)

*poItemIDArray*
:   Array of menu command IDs for which to get images

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmMenu5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5.html)

[IEdmMenu5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu5_members.html)

[IEdmMenu6::GetItems Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMenu6~GetItems.html)

# ![](dotnetimages/collapse.gif)Availability

Version 5.2 of SOLIDWORKS PDM Professional