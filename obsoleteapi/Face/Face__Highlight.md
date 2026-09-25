<!-- source: obsoleteapi/Face/Face__Highlight.htm -->

# Face::Highlight

This
method is obsolete and has been superseded by Face2::Highlight.

Description

This method highlights or de-highlights this face object.

Syntax (OLE Automation)

void
Face.Highlight ( state)

| Input: | (BOOL) state | TRUE highlights the face, FALSE de-highlights the face |

Syntax (COM)

status
= Face->IHighlight ( state )

| Input: | (VARIANT\_BOOL) state | TRUE highlights the face, FALSE de-highlights the face |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

The highlight state remains
in place until the model is rebuilt or redrawn.

SolidWorks does not support this method for faces obtained from reference
surface bodies.