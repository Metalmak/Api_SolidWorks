<!-- source: obsoleteapi/DrawingDoc/DrawingDoc__MakeBlockDefinition.htm -->

# DrawingDoc::MakeBlockDefinition

This
method is obsolete and has been superseded by SkethcManager::MakeSketchBlockFromFile,
SketchManager::MakeSketchBlockSelected,
and SketchManager::MakeSketchBlockFromSketch.

Description

This method makes a block definition from the
selected entities.

Syntax (OLE Automation)

retval = DrawingDoc.MakeBlockDefinition ( Name, XRefFileName,
Instance )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) Name | Block definition name |
| Input: | (BSTR) XRefFileName | Name of the file that the block definition references |
| Input: | (VARIANT\_BOOL) Instance | TRUE creates an instance, FALSE does not |
| Output: | (LPBLOCKDEFINITION) retval | Pointer to the new block definition |

Syntax (COM)

status = DrawingDoc->MakeBlockDefinition ( Name,
XRefFileName, Instance, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) Name | Block definition name |
| Input: | (BSTR) XRefFileName | Name of the file that the block definition references |
| Input: | (VARIANT\_BOOL) Instance | TRUE creates an instance, FALSE does not |
| Output: | (LPBLOCKDEFINITION) retval | Pointer to the new block definition |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This method is similar to
the DrawingDoc::CreateBlockDefinition method except that instead of creating
a block definition from the specified entities, DrawingDoc::MakeBlockDefinition
creates a block definition from the selected entities.

If you have the pointers to
the entities for the block definition, running DrawingDoc::CreateBlockDefinition
should be faster than selecting all of the entities and then running DrawingDoc::MakeBlockDefinition
because of the time spent having to select the entities.