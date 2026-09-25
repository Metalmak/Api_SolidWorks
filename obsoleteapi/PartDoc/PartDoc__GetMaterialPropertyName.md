<!-- source: obsoleteapi/PartDoc/PartDoc__GetMaterialPropertyName.htm -->

# PartDoc::GetMaterialPropertyName

This method is obsolete and has been superseded
by PartDoc::GetMaterialPropertyName2.

Description

This method gets the names
of the material database and the material.

Syntax (OLE Automation)

retval = PartDoc.GetMaterialPropertyName (\*database)

|  |  |  |
| --- | --- | --- |
| Output: | (BSTR \*) \*database | Name of material database |
| Output: | (BSTR\*) retval | Name of material |

#

Syntax (COM)

status = PartDoc->GetMaterialPropertyName ( \*database,
&retval)

|  |  |  |
| --- | --- | --- |
| Output: | (BSTR \*) \*database | Names of material database |
| Output: | (BSTR\*) retval | Name of material |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks

If no material was applied to the part, then database
and retval are blank.