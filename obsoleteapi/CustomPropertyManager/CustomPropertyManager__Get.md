<!-- source: obsoleteapi/CustomPropertyManager/CustomPropertyManager__Get.htm -->

# CustomPropertyManager::Get

This method is obsolete and has been superseded
by CustomPropertyManager::Get2.

Description

This method gets the value
of the specified custom property.

Syntax (OLE Automation)

retval = CustomPropertyManager.Get ( FieldName)

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) FieldName | Name of the custom property to get |
| Output: | (BSTR\*) retval | Value of custom property |

#

Syntax (COM)

status = CustomPropertyManager->Get ( FieldName,
&retval)

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) FieldName | Name of the custom property to get |
| Output: | (BSTR\*) retval | Value of custom property |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks