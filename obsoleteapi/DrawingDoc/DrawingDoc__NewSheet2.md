<!-- source: obsoleteapi/DrawingDoc/DrawingDoc__NewSheet2.htm -->

# DrawingDoc::NewSheet2

This method is obsolete and has been superseded
by DrawingDoc::NewSheet3.

Description

This method creates a new drawing sheet.

Syntax (OLE Automation)

retval = DrawingDoc.NewSheet2 ( name, paperSize,
templateIn, scale1, scale2, firstAngle, templateName, width, height)

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) name | Name to be given to the new sheet |
| Input: | (short) paperSize | Size of paper as defined in swDwgPaperSizes\_e |
| Input: | (short) templateIn | Template index as defined in swDwgTemplates\_e |
| Input: | (double) scale1 | Scale numerator |
| Input: | (double) scale2 | Scale denominator |
| Input: | (BOOL) firstAngle | TRUE for first angle projection, FALSE otherwise |
| Input: | (BSTR) templateName | Name of custom template with full directory path if templateIn = swDwgTemplateCustom |
| Input: | (double) width | Custom paper width if paperSize = swDwgPapersUserDefined |
| Input: | (double) height | Custom paper height if paperSize = swDwgPapersUserDefined |
| Return: | (BOOL) retval | TRUE if sheet creation was successful, FALSE if not |

Syntax (COM)

status = DrawingDoc->NewSheet2 ( name, paperSize,
templateIn, scale1, scale2, firstAngle, templateName, width, height, &retval
)

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) name | Name to be given to the new sheet |
| Input: | (short) paperSize | Size of paper as defined in swDwgPaperSizes\_e |
| Input: | (short) templateIn | Template index as defined in swDwgTemplates\_e |
| Input: | (double) scale1 | Scale numerator |
| Input: | (double) scale2 | Scale denominator |
| Input: | (VARIANT\_BOOL) firstAngle | TRUE for first angle projection, FALSE otherwise |
| Input: | (BSTR) templateName | Name of custom template with full directory path if templateIn = swDwgTemplateCustom |
| Input: | (double) width | Custom paper width if paperSize = swDwgPapersUserDefined |
| Input: | (double) height | Custom paper height if paperSize = swDwgPapersUserDefined |
| Output: | (VARIANT\_BOOL) retval | TRUE if sheet creation was successful, FALSE if not |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks

The templatetIn argument overrides the paperSize
argument if they do not match.