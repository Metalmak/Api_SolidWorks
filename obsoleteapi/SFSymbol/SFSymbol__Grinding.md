<!-- source: obsoleteapi/SFSymbol/SFSymbol__Grinding.htm -->

# SFSymbol::Grinding

This property is obsolete and has been superseded
by SFSymbol::GetSymbolSurfaceTexture.

Description

This property indicates whether or not grinding flag is set on this
surface-finish symbol.

Syntax (OLE Automation)

grinding
= SFSymbol.Grinding (VB Get property)

SFSymbol.Grinding
= grinding (VB Set property)

grinding
= SFSymbol.GetGrinding ( )  (C++ Get property)

SFSymbol.SetGrinding
( grinding )  (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (BOOL) grinding | TRUE if grinding flag is enabled, FALSE if disabled |

Syntax (COM)

status = SFSymbol->get\_Grinding ( &grinding
)

status = SFSymbol->put\_Grinding ( grinding )

|  |  |  |
| --- | --- | --- |
| Property: | (VARIANT\_BOOL) grinding | TRUE if grinding flag is enabled, FALSE if disabled |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks