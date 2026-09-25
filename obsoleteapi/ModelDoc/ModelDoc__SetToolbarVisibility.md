<!-- source: obsoleteapi/ModelDoc/ModelDoc__SetToolbarVisibility.htm -->

# ModelDoc::SetToolbarVisibility

This method is obsolete
and has been superseded by ModelDoc2::SetToolbarVisibility.

Description

This method sets the visibility of a toolbar.

Syntax (OLE Automation)

void ModelDoc.SetToolbarVisibility(
Toolbar, Visible )

|  |  |  |
| --- | --- | --- |
| Input: | (long) Toolbar | Identifier of toolbar as defined in swToolbar\_e |
| Input: | (BOOL) Visible | TRUE if the toolbar is to be visible, FALSE if it is hidden |

Syntax (COM)

status = ModelDoc->SetToolbarVisibility(
Toolbar , Visible)

|  |  |  |
| --- | --- | --- |
| Input: | (long) Toolbar | Identifier of toolbar as defined in swToolbar\_e |
| Input: | (VARIANT\_BOOL) Visible | TRUE if the toolbar is to be visible, FALSE if it is to be hidden |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks