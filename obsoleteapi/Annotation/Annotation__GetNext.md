<!-- source: obsoleteapi/Annotation/Annotation__GetNext.htm -->

# Annotation::GetNext

This
method is obsolete and has been superseded by [Annotation::GetNext2](Annotation__GetNext2.htm).

### Description

This method gets the next annotation object.

### Syntax (OLE Automation)

retval = Annotation.GetNext ()

| Return: | (LPDISPATCH) retval | Dispatch object of the next annotation |

### Syntax (COM)

status = Annotation->IGetNext (
&retval )

| Output: | (LPANNOTATION) retval | Pointer to the next annotation |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks