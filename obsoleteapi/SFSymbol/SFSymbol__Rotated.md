<!-- source: obsoleteapi/SFSymbol/SFSymbol__Rotated.htm -->

# SFSymbol::Rotated

This property is obsolete and has been superseded
by SFSymbol::Orientation.

Description

This property indicates whether this surface-finish symbol is horizontal
or vertical (rotated 90°).

Syntax (OLE Automation)

rotated = SFSymbol::Rotated (VB Get property)

SFSymbol::Rotated = rotated (VB Set property)

rotated = SFSymbol::GetRotated ( ) (C++ Get
property)

SFSymbol::SetRotated ( rotated ) (C++ Set property)

| Property: | (BOOL) rotated | TRUE if symbol is rotated 90° (vertical), FALSE if  symbol is not rotated (horizontal) |

Syntax (COM)

status = SFSymbol->Rotated ( VARIANT\_BOOL rotated
)

| Property: | (VARIANT\_BOOL) rotated | TRUE if symbol is rotated 90° (vertical), FALSE if  symbol is not rotated (horizontal) |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

To see the model or drawing changes caused by setting this property,
you must redraw your window. See ModelDoc2::GraphicsRedraw2 for details.