<!-- source: obsoleteapi/Configuration/Configuration__GetCustomPropertiesCount.htm -->

# Configuration::GetCustomPropertiesCount

This method is obsolete and has been superseded
by Configuration::CustomPropertyManager.

Description

This method gets the number of custom properties
in this configuration.

Syntax (OLE Automation)

numProps = Configuration.GetCustomPropertiesCount
( )

| Output: | (long) numProps | Number of properties |

Syntax (COM)

status = Configuration->GetCustomPropertiesCount
( &numProps )

| Output: | (long) numProps | Number of properties |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks