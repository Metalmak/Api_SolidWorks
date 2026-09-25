<!-- source: obsoleteapi/ModelDoc/ModelDoc__DeActivateFeatureMgrView.htm -->

# ModelDoc::DeActivateFeatureMgrView

This
method is obsolete and has been superseded by ModelDoc2::DeActivateFeatureMgrView.

Description

This method deactivates a tab in the FeatureManager
design tree view.

Syntax (OLE Automation)

retval = ModelDoc.DeActivateFeatureMgrView ( appView )

|  |  |  |
| --- | --- | --- |
| Input: | (long\*) appView | Pointer to the FeatureManager design tree view |
| Return: | (BOOL) retval | TRUE if deactivated, FALSE otherwise |

Syntax (COM)

status = ModelDoc->DeActivateFeatureMgrView (
appView, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (long\*) appView | Pointer to the FeatureManager design tree view |
| Output: | (VARIANT\_BOOL) retval | TRUE if deactivated, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks