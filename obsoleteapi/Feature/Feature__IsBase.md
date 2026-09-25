<!-- source: obsoleteapi/Feature/Feature__IsBase.htm -->

# Feature::IsBase

This method is obsolete and has been superseded
by Feature::IsBase2.

Description

This method determines whether this feature
is a base feature.

Syntax (OLE Automation)

bBase = Feature.IsBase ( )

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) bBase | TRUE if this is a base feature, FALSE if not |

Syntax (COM)

status = Feature->IsBase ( &bBase )

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) bBase | TRUE if this is a base feature, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks