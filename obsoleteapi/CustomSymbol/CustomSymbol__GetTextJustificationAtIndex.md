<!-- source: obsoleteapi/CustomSymbol/CustomSymbol__GetTextJustificationAtIndex.htm -->

# CustomSymbol::GetTextJustificationAtIndex

This method is obsolete and has been superseded
by Note::GetTextJustificationAtIndex.

Description

This method gets the justification of the specified
text item.

Syntax (OLE Automation)

retval = CustomSymbol.GetTextJustificationAtIndex
( index )

| Input: | (long) index | One-based index position of the text |
| Return: | (long) retval | Justification of the text as defined in swTextJustification\_e |

Syntax (COM)

status = CustomSymbol->GetTextJustificationAtIndex
( index, &retval )

| Input: | (long) index | One-based index position of the text |
| Output: | (long) retval | Justification of the text as defined in swTextJustification\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks