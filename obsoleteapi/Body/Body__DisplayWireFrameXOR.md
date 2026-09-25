<!-- source: obsoleteapi/Body/Body__DisplayWireFrameXOR.htm -->

# Body::DisplayWireFrameXOR

This method is obsolete and has been superseded by
Body2::DisplayWireFrameXOR.

Description

This method displays a temporary body in the given part's context in
XOR mode.

Syntax (OLE Automation)

void Body.DisplayWireFrameXOR ( part,
color)

|  |  |  |
| --- | --- | --- |
| Input: | (LPDISPATCH) part | Pointer to dispatch object, the part |
| Input: | (long) color | Desired color |

Syntax
(COM)

status = Body->IDisplayWireFrameXOR
( part, color )

|  |  |  |
| --- | --- | --- |
| Input: | (LPPARTDOC) part | Pointer to the part |
| Input: | (long) color | Desired color |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks