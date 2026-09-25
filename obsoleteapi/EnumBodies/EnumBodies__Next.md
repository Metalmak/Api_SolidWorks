<!-- source: obsoleteapi/EnumBodies/EnumBodies__Next.htm -->

# EnumBodies::Next

This method is obsolete and has been superseded by
EnumBodies2::Next.

Description

This method gets the next body.

Syntax (OLE Automation)

Not available.

Syntax (COM)

status = EnumBodies->Next ( celt,
&rgelt, pceltFetched )

| Input: | (long) celt | Number bodies desired for the enumerated list |
| Output: | (LPBODY) rgelt | Pointer to the enumerated list of bodies |
| Output: | (long\*) pceltFetched | Pointer to the number of bodies returned from the list; this value could be less than celt if you asked for more bodies than exist, or it could be NULL if no more bodies exist |
| Return: | (HRESULT) status | S\_OK if successful |