<!-- source: obsoleteapi/Configuration/Configuration__Select.htm -->

# Configuration::Select

This method is obsolete and has been superseded
by Configuration::Select2.

Description

This method selects the configuration.

Syntax (OLE Automation)

retval = Configuration.Select ( appendFlag)

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT\_BOOL) appendFlag | TRUE appends the configuration to the selection list, FALSE replaces the selection list with the configuration |
| Output: | (VARIANT\_BOOL) retval | TRUE if the configuration is selected, FALSE if not |

#

Syntax (COM)

status = Configuration->Select ( appendFlag, &retval)

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT\_BOOL) appendFlag | TRUE appends the configuration to the selection list, FALSE replaces the selection list with the configuration |
| Output: | (VARIANT\_BOOL) retval | TRUE if the configuration is selected, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks