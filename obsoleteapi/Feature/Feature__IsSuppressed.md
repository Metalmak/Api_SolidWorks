<!-- source: obsoleteapi/Feature/Feature__IsSuppressed.htm -->

# Feature::IsSuppressed

This method is obsolete and has been superseded
by Feature::IsSuppressed2.

Description

This
method determines whether or not the feature is suppressed.

Syntax (OLE Automation)

retval
= Feature.IsSuppressed ()

|  |  |  |
| --- | --- | --- |
| Return: | (VARIANT\_BOOL) retval | TRUE if this feature is suppressed, FALSE if it is not |

Syntax (COM)

status = Feature->IsSuppressed (
&retval )

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if this feature is suppressed, FALSE if it is not |
| Return: | (HRESULT) -  status | S\_OK if successful |