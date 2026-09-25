<!-- source: obsoleteapi/ModelDoc/ModelDoc__FontBold.htm -->

# ModelDoc::FontBold

This method is obsolete
and has been superseded by ModelDoc2::FontBold.

Description

This method enables or disables bold font style
in the selected notes, dimensions, and Gtols.

Syntax (OLE Automation)

(void) ModelDoc.FontBold
( bold )

|  |  |  |
| --- | --- | --- |
| Input: | (BOOL) bold | If TRUE, then bold font style is enabled, if FALSE, then bold font style is disabled |

Syntax (COM)

status = ModelDoc->FontBold
( bold )

| Input: | (VARIANT\_BOOL) bold | If TRUE, then bold font style is enabled, if FALSE, then bold font style is disabled |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

See the TextFormat object for full control of text
formatting. You can obtain this object using the GetTextFormat interfaces.