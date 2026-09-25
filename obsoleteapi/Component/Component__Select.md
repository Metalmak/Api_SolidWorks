<!-- source: obsoleteapi/Component/Component__Select.htm -->

# Component::Select

This method is obsolete and has been superseded by
[Component2::Select](../Component2/Component2__Select.htm).

Description

This method selects the component and either
appends it to the selections or replaces the entire selection list.

Syntax (OLE Automation)

retval = Component.Select ( appendFlag )

| Input: | (BOOL) appendFlag | TRUE appends the current selection list, FALSE replaces the selection list |
| Return: | (BOOL) retval | TRUE if the feature was selected, FALSE if it was not |

Syntax (COM)

status = Component->Select ( appendFlag, &retval
)

| Input: | (VARIANT\_BOOL) appendFlag | TRUE appends the current selection list, FALSE replaces the selection list |
| Output: | (VARIANT\_BOOL) retval | TRUE if the feature was selected, FALSE if it was not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks