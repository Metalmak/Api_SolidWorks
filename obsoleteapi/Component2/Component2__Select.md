<!-- source: obsoleteapi/Component2/Component2__Select.htm -->

# Component2::Select

This
method is obsolete and has been superseded by [Component2::Select2](Component2__Select2.htm).

Description

This method selects the component and appends
it to the selections or replaces the entire selection list.

Syntax (OLE Automation)

retval = Component2.Select ( appendFlag )

| Input: | (BOOL) appendFlag | TRUE appends the selection list, FALSE replaces the selection list |
| Return: | (BOOL) retval | TRUE if the feature was selected, FALSE if not |

Syntax (COM)

status = Component2->Select ( appendFlag, &retval
)

| Input: | (VARIANT\_BOOL) appendFlag | TRUE appends the selection list, FALSE replaces the selection list |
| Output: | (VARIANT\_BOOL) retval | TRUE if the feature was selected, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Use [ModelDoc2::SelectByID](../ModelDoc2/ModelDoc2__SelectByID.htm)
instead of using this method. This method does not work well when a PropertyManager
page is open or a command is running. ModelDoc2::SelectByID handles selection
correctly whether or not a command is running.