<!-- source: obsoleteapi/SldWorks/SldWorks__PreSelectDwgTemplateSize.htm -->

# SldWorks::PreSelectDwgTemplateSize

This method is obsolete and has been superseded
by SldWorks::PresetNewDrawingParameters
and SldWorks::ResetPresetDrawingParameters.

Description

This method establishes which template to use when creating a drawing.
By calling this method and specifying a template size, no dialog appears
when the end-user interactively selects File,
New, Drawing.

Syntax (OLE Automation)

void SldWorks.PreSelectDwgTemplateSize
( templateToUse, templateName)

|  |  |  |
| --- | --- | --- |
| Input: | (long) templateToUse | Type of template to use as defined in swDwgTemplates\_e |
| Input: | (BSTR) templateName | Reserved for future use; use NULL |

Syntax (COM)

status = SldWorks->PreSelectDwgTemplateSize
( templateToUse, templateName )

|  |  |  |
| --- | --- | --- |
| Input: | (long) templateToUse | Type of template to use as defined in swDwgTemplates\_e |
| Input: | (BSTR) templateName | Reserved for future use; use NULL |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks