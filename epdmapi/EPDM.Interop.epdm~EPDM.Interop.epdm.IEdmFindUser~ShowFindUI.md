<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser~ShowFindUI.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| ShowFindUI Method (IEdmFindUser) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmFindUser Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser.html) : ShowFindUI Method (IEdmFindUser) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lParentWnd*
:   Parent window handle of the search dialog box

*bAllowMultiSelect*
:   True to permit the user to select more than one user in the search result, false to not

*bsCaption*
:   Caption for the dialog box; "" to use the default, localized caption

Displays the Find User dialog box so the user can enter search criteria and select users from the result list.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function ShowFindUI( _    ByVal lParentWnd As System.Integer, _    ByVal bAllowMultiSelect As System.Boolean, _    Optional ByVal bsCaption As System.String _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ShowFindUI(     System.int lParentWnd,    System.bool bAllowMultiSelect,    System.string bsCaption ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ShowFindUI(  &   System.int lParentWnd, &   System.bool bAllowMultiSelect, &   System.String^ bsCaption ) ``` | |

#### Parameters

*lParentWnd*
:   Parent window handle of the search dialog box

*bAllowMultiSelect*
:   True to permit the user to select more than one user in the search result, false to not

*bsCaption*
:   Caption for the dialog box; "" to use the default, localized caption

#### Return Value

True if a user is selected in the search result, false if the dialog box is canceled

# ![](dotnetimages/collapse.gif)Example

See the [IEdmFindUser](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [IEdmFindUser::SetPropt](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser~SetPropt.html) to set the search criteria for finding users. The search criteria become the default values in the Find User dialog box that is launched when this method is called.

After successfully calling this method, the [IEdmFindUser.Result](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser~Result.html) property contains the users selected in the result list of the Find User dialog box.

SOLIDWORKS PDM Professional calls this function when you link a card button to the Find User command.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: An argument is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmFindUser Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser.html)

[IEdmFindUser Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmFindUser_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013