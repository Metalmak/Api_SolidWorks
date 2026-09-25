<!-- source: obsoleteapi/SFSymbol/SFSymbol__SetSymbolType.htm -->

# SFSymbol::SetSymbolType

This method is obsolete and has been superseded
by SFSymbol::SetSymbol.

Description

This method sets the symbol type for this surface-finish symbol.

Syntax (OLE Automation)

retval = SFSymbol.SetSymbolType (
symbolType )

|  |  |  |
| --- | --- | --- |
| Input: | (long) symbolType | Symbol type as defined in swSFSymType\_e |
| Return: | (BOOL) retval | TRUE if the symbol type is successfully set, FALSE if not |

Syntax (COM)

status = SFSymbol->SetSymbolType ( symbolType,
&retval )

|  |  |  |
| --- | --- | --- |
| Input: | (long) symbolType | Symbol type as defined in swSFSymType\_e |
| Output: | (VARIANT\_BOOL) retval | TRUE if the symbol type is successfully set, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

If an invalid symbol type is specified, the symbol
is not changed, and FALSE is returned.

To see the model or drawing changes caused by running
this method, you must redraw your window. See ModelDoc2::GraphicsRedraw2
for details.

To get the symbol type, use SFSymbol::GetSymbolType.