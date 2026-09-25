<!-- source: obsoleteapi/DrawingDoc/DrawingDoc__ExplodeBlockInstance.htm -->

# DrawingDoc::ExplodeBlockInstance

This method is obsolete and has been superseded
by SketchManager::ExplodeSketchBlockInstance.

Description

This method explodes the selected
block instances into individual entities.

Syntax (OLE Automation)

retval = DrawingDoc.ExplodeBlockInstance ( )

#

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if the block instance is exploded, FALSE if not |

#

Syntax (COM)

status = DrawingDoc->ExplodeBlockInstance ( &retval
)

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if the block instance is exploded, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks