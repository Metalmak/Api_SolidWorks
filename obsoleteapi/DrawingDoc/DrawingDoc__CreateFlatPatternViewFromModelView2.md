<!-- source: obsoleteapi/DrawingDoc/DrawingDoc__CreateFlatPatternViewFromModelView2.htm -->

# DrawingDoc::CreateFlatPatternViewFromModelView2

This method is obsolete and has been superseded
by DrawingDoc::CreateFlatPatternViewFromModelView3.

Description

This method creates a flat-pattern view from
a model view.

Syntax (OLE Automation)

retval = DrawingDoc.CreateFlatPatternViewFromModelView2
( modelName, configName, locX, locY, locZ, hideBendLines )

| Input: | (BSTR) modelName | Name of model |
| Input: | (BSTR) configName | Name of configuration |
| Input: | (double) locX | X coordinate |
| Input: | (double) locY | Y coordinate |
| Input: | (double) locZ | Z coordinate |
| Input: | (VARIANT\_BOOL) hideBendLines | TRUE hides bend lines, FALSE does not |
| Output: | (VARIANT\_BOOL) retval | TRUE if the flat-pattern view was created successfully, FALSE if it was not |

Syntax (COM)

status = DrawingDoc->CreateFlatPatternViewFromModelView2
( modelName, configName, locX, locY, locZ, hideBendLines, &retval
)

| Input: | (BSTR) modelName | Name of model |
| Input: | (BSTR) configName | Name of configuration |
| Input: | (double) locX | X coordinate |
| Input: | (double) locY | Y coordinate |
| Input: | (double) locZ | Z coordinate |
| Input: | (VARIANT\_BOOL) hideBendLines | TRUE hides bend lines, FALSE does not |
| Output: | (VARIANT\_BOOL) retval | TRUE if the flat-pattern view was created successfully, FALSE if it was not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks