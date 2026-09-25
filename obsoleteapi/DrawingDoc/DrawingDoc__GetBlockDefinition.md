<!-- source: obsoleteapi/DrawingDoc/DrawingDoc__GetBlockDefinition.htm -->

# DrawingDoc::GetBlockDefinition

This method is obsolete and has been superseded
by SketchManager::GetSketchBlockDefinitions.

Description

This method gets the specified block definition.

Syntax (OLE Automation)

retval = DrawingDoc.GetBlockDefinition ( Name )

| Input: | (BSTR) Name | Block definition name |
| Output: | (LPBLOCKDEFINITION) retval | Pointer to the block definition |

Syntax (COM)

status = DrawingDoc->GetBlockDefinition ( Name,
&retval )

| Input: | (BSTR) Name | Block definition name |
| Output: | (LPBLOCKDEFINITION) retval | Pointer to the block definition |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks