<!-- source: obsoleteapi/ModelDoc/ModelDoc__Toolbars.htm -->

# ModelDoc::Toolbars

This
method is obsolete and has been superseded by ModelDoc2::Toolbars.

Description

This method turns the main SolidWorks toolbars on and off.

Syntax (OLE Automation)

void ModelDoc.Toolbars ( m, vw, skMain,
sk, feat, constr, macro)

|  |  |  |
| --- | --- | --- |
| Input: | (BOOL) m | TRUE for main toolbar on, FALSE for off |
| Input: | (BOOL) vw | TRUE for view manipulation toolbar on, FALSE for off |
| Input: | (BOOL) skMain | TRUE for main sketch toolbar on, FALSE for off |
| Input: | (BOOL) sk | TRUE for sketch entity toolbar on, FALSE for off |
| Input: | (BOOL) feat | TRUE for feature toolbar on, FALSE for off |
| Input: | (BOOL) constr | TRUE for relationships toolbar on, FALSE for off |
| Input: | (BOOL) macro | TRUE for macro toolbar on, FALSE for off |

Syntax (COM)

status = ModelDoc->Toolbars ( m,
vw, skMain, sk, feat, constr, macro )

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT\_BOOL) m | TRUE for main toolbar on, FALSE for off |
| Input: | (VARIANT\_BOOL) vw | TRUE for view manipulation toolbar on, FALSE for off |
| Input: | (VARIANT\_BOOL) skMain | TRUE for main sketch toolbar on, FALSE for off |
| Input: | (VARIANT\_BOOL) sk | TRUE for sketch entity toolbar on, FALSE for off |
| Input: | (VARIANT\_BOOL) feat | TRUE for feature toolbar on, FALSE for off |
| Input: | (VARIANT\_BOOL) constr | TRUE for relationships toolbar on, FALSE for off |
| Input: | (VARIANT\_BOOL) macro | TRUE for macro toolbar on, FALSE for off |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

See ModelDoc.SetToolbarVisibility for control of all SolidWorks toolbars.