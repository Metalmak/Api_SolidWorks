<!-- source: obsoleteapi/ModelDoc2/ModelDoc2__DeleteConfiguration.htm -->

# ModelDoc2::DeleteConfiguration

This
method is obsolete and has been superseded by ModelDoc2::DeleteConfiguration2.

Description

This method deletes a configuration. The configuration cannot be the
active configuration.

Syntax (OLE Automation)

void ModelDoc2.DeleteConfiguration
( configurationName)

| Input: | (BSTR) configurationName | Name of the configuration to delete |

Syntax (COM)

status = ModelDoc2->DeleteConfiguration
( configurationName )

| Input: | (BSTR) configurationName | Name of the configuration to delete |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks