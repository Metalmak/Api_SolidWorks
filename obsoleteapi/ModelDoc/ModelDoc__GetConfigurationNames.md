<!-- source: obsoleteapi/ModelDoc/ModelDoc__GetConfigurationNames.htm -->

# ModelDoc::GetConfigurationNames

This
method is obsolete and has been superseded by ModelDoc2::GetConfigurationNames.

Description

This method returns a list of configuration names existing in this document.

Syntax (OLE Automation)

retval = ModelDoc.GetConfigurationNames(
)

|  |  |  |
| --- | --- | --- |
| Return: | (VARIANT) retval | VARIANT of type SafeArray of the names of the configurations in this part |

Syntax (COM)

status = ModelDoc->IGetConfigurationNames(
&configCount, configList )

|  |  |  |
| --- | --- | --- |
| In/Out: | (long) configCount | Number of configurations in this part |
| Output: | (BSTR) configList | Array of the names of the configurations in this part of size configCount |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

 ModelDoc::GetConfigurationCount
before calling this method.