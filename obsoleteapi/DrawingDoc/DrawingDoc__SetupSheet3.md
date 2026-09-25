<!-- source: obsoleteapi/DrawingDoc/DrawingDoc__SetupSheet3.htm -->

# DrawingDoc::SetupSheet3

This method is obsolete and has been superseded
by DrawingDoc::SetupSheet4.

Description

This method changes the settings for the current sheet on this drawing
document.

Syntax (OLE Automation)

retval = DrawingDoc.SetupSheet3 ( name, paperSize,
templateIn, scale1, scale2, firstAngle, templateName, width, height )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) name | Name for the sheet |
| Input: | (long) paperSize | Size of paper as defined in swDwgPaperSizes\_e |
| Input: | (long) templateIn | Template index as defined in swDwgTemplates\_e |
| Input: | (double) scale1 | Scale numerator |
| Input: | (double) scale2 | Scale denominator |
| Input: | (BOOL)firstAngle | TRUE for first angle projection, FALSE otherwise |
| Input: | (BSTR) templateName | Name of custom template with full directory path if templateIn = swDwgTemplateCustom |
| Input: | (double) width | Custom paper width if paperSize = swDwgPapersUserDefined |
| Input: | (double) height | Custom paper height if paperSize = swDwgPapersUserDefined |
| Return: | (BOOL)retval | TRUE if successful, FALSE if not |

Syntax (COM)

status = DrawingDoc->SetupSheet3
( name, paperSize, templateIn, scale1, scale2, firstAngle, templateName,
width, height, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR)name | Name for the sheet |
| Input: | (long)paperSize | Size of paper as defined in swDwgPaperSizes\_e |
| Input: | (long)templateIn | Template index as defined in swDwgTemplates\_e |
| Input: | (double)scale1 | Scale numerator |
| Input: | (double)scale2 | Scale denominator |
| Input: | (VARIANT\_BOOL)firstAngle | TRUE for first angle projection, FALSE otherwise |
| Input: | (BSTR)templateName | Name of custom template with full directory path if templateIn = swDwgTemplateCustom |
| Input: | (double)width | Custom paper width if paperSize = swDwgPapersUserDefined |
| Input: | (double)height | Custom paper height if paperSize = swDwgPapersUserDefined |
| Output: | (VARIANT\_BOOL)retval | TRUE if successful, FALSE if not |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks

You can also use Sheet::SetProperties, Sheet::SetName, and Sheet::SetTemplateName.

The templateIn value overrides paperSize if they do not match.