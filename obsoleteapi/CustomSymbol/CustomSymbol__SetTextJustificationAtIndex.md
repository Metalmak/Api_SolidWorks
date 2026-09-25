<!-- source: obsoleteapi/CustomSymbol/CustomSymbol__SetTextJustificationAtIndex.htm -->

# CustomSymbol::SetTextJustificationAtIndex

This method is obsolete and has been superseded
by Note::SetTextJustificationAtIndex.

Description

This method sets the justification of the specified
text item.

Syntax (OLE Automation)

void CustomSymbol.SetTextJustificationAtIndex ( index,
justification)

| Input: | (long) index | One-based index position of the text |
| Input: | (long) justification | Justification of the text as defined in swTextJustification\_e |

Syntax (COM)

status = CustomSymbol->SetTextJustificationAtIndex
( index, justification )

| Input: | (long) index | One-based index position of the text |
| Input: | (long) justification | Justification of the text as defined in swTextJustification\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks