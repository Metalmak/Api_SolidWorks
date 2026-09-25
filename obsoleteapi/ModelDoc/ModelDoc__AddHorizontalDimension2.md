<!-- source: obsoleteapi/ModelDoc/ModelDoc__AddHorizontalDimension2.htm -->

# ModelDoc::AddHorizontalDimension2

This
method is obsolete and has been superseded by ModelDoc2::AddHorizontalDimension2.

Description

This method creates a horizontal dimension
for the current selected entities at the specified location.

Syntax (OLE Automation)

retval = ModelDoc.AddHorizontalDimension2 ( x, y,
z )

|  |  |  |
| --- | --- | --- |
| Input: | (double) x | Dimension text location, in meters |
| Input: | (double) y | Dimension text location, in meters |
| Input: | (double) z | Dimension text location, in meters |
| Return: | (LPDISPATCH) retval | A pointer to the newly created dimension |

Syntax (COM)

status = ModelDoc->IAddHorizontalDimension2 (
x, y, z, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (double) x | Dimension text location, in meters |
| Input: | (double) y | Dimension text location, in meters |
| Input: | (double) z | Dimension text location, in meters |
| Output: | (LPDISPLAYDIMENSION) retval | A pointer to the newly created dimension |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks