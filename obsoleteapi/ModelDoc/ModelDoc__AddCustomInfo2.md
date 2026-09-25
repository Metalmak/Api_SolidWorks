<!-- source: obsoleteapi/ModelDoc/ModelDoc__AddCustomInfo2.htm -->

# ModelDoc::AddCustomInfo2

This
method is obsolete and has been superseded by [ModelDoc::AddCustomInfo3](ModelDoc__AddCustomInfo3.htm).

Description

This method adds a custom property field to the document.

Syntax (OLE Automation)

retval = ModelDoc.AddCustomInfo2(
FieldName, FieldType, FieldValue )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) FieldName | Name of custom property |
| Input: | (long) FieldType | Type of custom property as defined in swCustomInfoType\_e |
| Input: | (BSTR) FieldValue | Value of custom property |
| Return: | (BOOL) retval | TRUE if added, FALSE if not |

Syntax (COM)

status = ModelDoc->AddCustomInfo2(
FieldName, FieldType, FieldValue, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) FieldName | Name of custom property |
| Input: | (long) FieldType | Type of custom property as defined in swCustomInfoType\_e |
| Input: | (BSTR) FieldValue | Value of custom property |
| Output: | (VARIANT\_BOOL) retval | TRUE if added, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks