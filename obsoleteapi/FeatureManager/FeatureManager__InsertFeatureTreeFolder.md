<!-- source: obsoleteapi/FeatureManager/FeatureManager__InsertFeatureTreeFolder.htm -->

# FeatureManager::InsertFeatureTreeFolder

This method is obsolete and has been superseded
by FeatureManager::InsertFeatuerTreeFolder2.

Description

This method inserts a folder
in the FeatureManager design tree.

Syntax (OLE Automation)

retval = FeatureManager.InsertFeatureTreeFolder (
)

#

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if the folder is created and inserted, FALSE if not |

#

Syntax (COM)

status = FeatureManager->InsertFeatureTreeFolder
( &retval )

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if the folder is created and inserted, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks