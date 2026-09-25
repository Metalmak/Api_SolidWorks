<!-- source: obsoleteapi/DrawingDoc/DrawingDoc__GetEditBlock.htm -->

# DrawingDoc::GetEditBlock

This method is obsolete and has been superseded
by SketchManager::EditSketchBlock
and SketchManager::EndEditSketchBlock.

Description

This method gets whether or
not a block is being edited in the drawing.

Syntax (OLE Automation)

retval = DrawingDoc.GetEditBlock ()

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if a block is being edited, FALSE if not |

#

Syntax (COM)

status = DrawingDoc->GetEditBlock ( &retval)

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if a block is being edited, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks