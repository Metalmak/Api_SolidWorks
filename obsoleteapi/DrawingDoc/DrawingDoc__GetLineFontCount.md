<!-- source: obsoleteapi/DrawingDoc/DrawingDoc__GetLineFontCount.htm -->

# DrawingDoc::GetLineFontCount

This
method is obsolete and has been superseded by DrawingDoc::GetLineFontCount2.

Description

This method gets the a number of line fonts supported by this drawing.

Syntax (OLE Automation)

retval
= DrawingDoc.GetLineFontCount ()

| Return: | (long) retval | Number of line fonts supported by this drawing |

Syntax (COM)

status
= DrawingDoc->GetLineFontCount ( &retval )

| Output: | (long) retval | Number of line fonts supported by this drawing |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Each line style is identified by an index
in the range [0, (retval -1) ].