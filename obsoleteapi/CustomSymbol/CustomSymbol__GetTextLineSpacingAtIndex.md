<!-- source: obsoleteapi/CustomSymbol/CustomSymbol__GetTextLineSpacingAtIndex.htm -->

# CustomSymbol::GetTextLineSpacingAtIndex

This method is obsolete and has been superseded
by Note::GetTextLineSpacingAtIndex.

Description

This method gets the line spacing for the specified
text item.

Syntax (OLE Automation)

retval = CustomSymbol.GetTextLineSpacingAtIndex (
index )

| Input: | (long) index | One-based index position of the text |
| Return: | (double) retval | Line spacing |

Syntax (COM)

status = CustomSymbol->GetTextLineSpacingAtIndex
( index, &retval )

| Input: | (long) index | One-based index position of the text |
| Output: | (double) retval | Line spacing |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks