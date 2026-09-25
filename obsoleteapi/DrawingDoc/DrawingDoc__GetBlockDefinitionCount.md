<!-- source: obsoleteapi/DrawingDoc/DrawingDoc__GetBlockDefinitionCount.htm -->

# DrawingDoc::GetBlockDefinitionCount

This method is obsolete and has been superseded
by SketchManager::GetSketchBlockDefinitionCount.

Description

This method gets the number of block definitions
in this drawing.

Syntax (OLE Automation)

retval = DrawingDoc.GetBlockDefinitionCount ( )

| Output: | (long) retval | Number of block definitions |

Syntax (COM)

status = DrawingDoc->GetBlockDefinitionCount (
&retval )

| Output: | (long) retval | Number of block definitions |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks