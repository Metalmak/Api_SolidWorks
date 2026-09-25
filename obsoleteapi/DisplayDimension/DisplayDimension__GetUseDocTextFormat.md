<!-- source: obsoleteapi/DisplayDimension/DisplayDimension__GetUseDocTextFormat.htm -->

# DisplayDimension::GetUseDocTextFormat

This method is obsolete and has been superseded
by Annotation::GetUseDocTextFormat.

Description

This method gets whether or not the default dimension text format is
used in this document.

Syntax (OLE Automation)

retval = DisplayDimension.GetUseDocTextFormat
( )

| Return: | (BOOL)retval | TRUE if the documents text formatting is used, FALSE otherwise |

Syntax (COM)

status = DisplayDimension->GetUseDocTextFormat
( &retval )

| Output: | (VARIANT\_BOOL) retval | TRUE if the documents text formatting is used, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks