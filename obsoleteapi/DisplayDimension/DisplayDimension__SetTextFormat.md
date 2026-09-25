<!-- source: obsoleteapi/DisplayDimension/DisplayDimension__SetTextFormat.htm -->

# DisplayDimension::SetTextFormat

This method is obsolete and has been superseded
by Annotation::SetTextFormat.

Description

This
method sets the text format parameters for this display dimension.

Syntax (OLE Automation)

retval
= DisplayDimension.SetTextFormat ( textFormatType, textFormat )

| Input: | (long) textFormatType | Determines whether the dimension uses the document text format or the textFormat argument values |
| Input: | (LPDISPATCH) textFormat | Formatting values |
| Return: | (BOOL) retval | TRUE if successfully set, FALSE if not |

Syntax (COM)

status
= DisplayDimension->ISetTextFormat ( textFormatType, textFormat, &retval
)

| Input: | (long) textFormatType | Determines whether the dimension uses the document text format or the textFormat argument values |
| Input: | (LPTEXTFORMAT) textFormat | Formatting values |
| Output: | (VARIANT\_BOOL) retval | TRUE if successfully set, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This method sets the text formatting for the dimension to the document
text formatting if useDocFormat is 1, or the formatting specified in the
textFormat argument if useDocFormat
is 0.