<!-- source: obsoleteapi/ModelDoc2/ModelDoc2__EditRollback2.htm -->

# ModelDoc2::EditRollback2

This method is obsolete and has been superseded
by FeatureManager::EditRollback.

Description

This method rolls back the FeatureManager design
tree's rollback bar to just before the selected feature.

Syntax (OLE Automation)

retval = ModelDoc2.EditRollback2 ( )

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if rollback successful, FALSE otherwise |

Syntax (COM)

status = ModelDoc2->EditRollback2 ( &retval
)

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if rollback successful, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

The selected feature, and those below it in the
FeatureManager design tree, are  suppressed
and unaccessible.

This routine is identical to ModelDoc2::EditRollback.
The version number was incremented to allow VB applications to take advantage
of information not available in PartDoc::EditRollback.