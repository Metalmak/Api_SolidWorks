<!-- source: obsoleteapi/Feature/Feature__Select.htm -->

# Feature::Select

This
method is obsolete and has been superseded by Feature::Select2.

Description

This method selects the feature and either
appends it to the selections or replaces the entire selection list.

Syntax (OLE Automation)

retval = Feature.Select ( appendFlag )

| Input: | (BOOL) appendFlag | TRUE appends the feature to the current selection list, FALSE replaces the current selection list |
| Return: | (BOOL) retval | TRUE if the feature was selected, FALSE if not |

Syntax (COM)

status = Feature->Select ( appendFlag, &retval
)

| Input: | (VARIANT\_BOOL) appendFlag | TRUE appends the feature to the current selection list, FALSE replaces the current selection list |
| Output: | (VARIANT\_BOOL) retval | TRUE if the feature was selected, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Use [ModelDoc2::SelectByID](../ModelDoc2/ModelDoc2__SelectByID.htm)
instead of this method. This method does not work well when a PropertyManager
page is open or a command is running. ModelDoc2::SelectByID handles selection
correctly whether or not a command is running.