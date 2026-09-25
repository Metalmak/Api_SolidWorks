<!-- source: obsoleteapi/ModelDoc/ModelDoc__GetToolbarVisibility.htm -->

# ModelDoc::GetToolbarVisibility

This
method is obsolete and has been superseded by ModelDoc2::GetToolbarVisibility.

Description

This method gets
the visibility of a toolbar.

Syntax (OLE Automation)

Visible = ModelDoc.GetToolbarVisibility(
Toolbar )

|  |  |  |
| --- | --- | --- |
| Input: | (long) Toolbar | Identifier of toolbar as defined in swToolbar\_e |
| Return: | (BOOL) Visible | TRUE if the toolbar is visible, FALSE if it is hidden |

Syntax (COM)

status = ModelDoc->GetToolbarVisibility(
Toolbar , &Visible)

|  |  |  |
| --- | --- | --- |
| Input: | (long) Toolbar | Identifier of toolbar as defined in swToolbar\_e |
| Output: | (VARIANT\_BOOL) Visible | TRUE if the toolbar is visible, FALSE if it is hidden |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks