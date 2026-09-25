<!-- source: obsoleteapi/ModelDoc/ModelDoc__FontItalic.htm -->

# ModelDoc::FontItalic

This
method is obsolete and has been superseded by ModelDoc2::FontItalic.

Description

This method enables or disables the Italic font
style in the selected notes, dimensions, and Gtols.

Syntax (OLE Automation)

(void) ModelDoc.FontItalic
( italic )

|  |  |  |
| --- | --- | --- |
| Input: | (Boolean) italic | If TRUE, then Italic style is enabled, if FALSE, then Italic is disabled |

Syntax (COM)

status = ModelDoc->FontItalic
( italic )

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT\_BOOL) italic | If TRUE, then Italic style is enabled, if FALSE, then Italic is disabled |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

You can also refer to the TextFormat object for
full control of text formatting. You can obtain this object by using the
GetTextFormat interfaces.