<!-- source: obsoleteapi/ModelDoc/ModelDoc__GetNext.htm -->

# ModelDoc::GetNext

This
method is obsolete and has been superseded by ModelDoc2::GetNext.

Description

This method gets
the next document in the current SolidWorks session.

Syntax (OLE Automation)

nextDoc = ModelDoc.GetNext
( )

|  |  |  |
| --- | --- | --- |
| Return: | (LPDISPATCH) nextDoc | Pointer to a Dispatch object, the next ModelDoc object |

Syntax (COM)

status = ModelDoc->IGetNext
( &nextDoc )

|  |  |  |
| --- | --- | --- |
| Output: | (LPMODELDOC) nextDoc | Pointer to the next ModelDoc object |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

The COM version of this method
is available in [datecode](../SldWorks/SldWorks__DateCode.htm) 1999/207 and later.