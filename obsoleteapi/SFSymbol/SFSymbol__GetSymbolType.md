<!-- source: obsoleteapi/SFSymbol/SFSymbol__GetSymbolType.htm -->

# SFSymbol::GetSymbolType

This method is obsolete and has been superseded
by SFSymbol::GetSymbol.

Description

This method gets the symbol type for this surface-finish symbol.

Syntax (OLE Automation)

retval = SFSymbol.GetSymbolType ( )

|  |  |  |
| --- | --- | --- |
| Return: | (long) retval | Symbol type as defined in swSFSymType\_e |

Syntax (COM)

status = SFSymbol->GetSymbolType ( &retval
)

|  |  |  |
| --- | --- | --- |
| Output: | (long) retval | Symbol type as defined in swSFSymType\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

To set the symbol type, use SFSymbol::SetSymbolType.