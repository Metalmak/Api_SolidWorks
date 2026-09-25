<!-- source: obsoleteapi/CustomSymbol/CustomSymbol__IsAttached.htm -->

# CustomSymbol::IsAttached

This method is obsolete and has been superseded
by Note::IsAttached.

Description

This
method determines if this symbol is attached.

Syntax (OLE Automation)

retval
= CustomSymbol.IsAttached ( )

| Return: | (BOOL) retval | TRUE if a leaderline is associated with this symbol, FALSE if not |

Syntax (COM)

status = CustomSymbol->IsAttached
( &retval )

| Output: | (VARIANT\_BOOL) retval | TRUE if a leaderline is associated with this symbol, FALSE if not |
| Return: | (HRESULT) status | S\_OK if Successful |