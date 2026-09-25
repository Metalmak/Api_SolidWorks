<!-- source: obsoleteapi/ModelDoc2/ModelDoc2__InsertWeldSymbol2.htm -->

# ModelDoc2::InsertWeldSymbol2

This method is obsolete and has been superseded
by ModelDoc2::InsertWeldSymbol3.

Description

This method creates a weld symbol on the last
edge selection.

Syntax (OLE Automation)

ModelDoc2.InsertWeldSymbol2 ( dim1, symbol, dim2,
symmetric, fieldWeld, showOtherSide, dashOnTop, peripheral, hasProcess,
processValue )

#

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) dim1 | First text value to the left of the symbol |
| Input: | (BSTR) symbol | Weld symbol name |
| Input: | (BSTR) dim2 | Text value to the right of the symbol |
| Input: | (VARIANT\_BOOL) symmetric | TRUE puts the symbol both above and below the horizontal line |
| Input: | (VARIANT\_BOOL) fieldWeld | TRUE puts a flag for field welding |
| Input: | (VARIANT\_BOOL) showOtherSide | Not used; pass 0 |
| Input: | (VARIANT\_BOOL) dashOnTop | TRUE puts the dash line on top |
| Input: | (VARIANT\_BOOL) peripheral | TRUE puts a peripheral symbol |
| Input: | (VARIANT\_BOOL) hasProcess | TRUE to specify a processValue |
| Input: | (BSTR) processValue | Process value if hasProcess is set to TRUE |

Syntax (COM)

status = ModelDoc2->InsertWeldSymbol2 ( dim1,
symbol, dim2, symmetric, fieldWeld, showOtherSide, dashOnTop, peripheral,
hasProcess, processValue )

| Input: | (BSTR) dim1 | First text value to the left of the symbol |
| Input: | (BSTR) symbol | Weld symbol name |
| Input: | (BSTR) dim2 | Text value to the right of the symbol |
| Input: | (VARIANT\_BOOL) symmetric | TRUE puts the symbol both above and below the horizontal line |
| Input: | (VARIANT\_BOOL) fieldWeld | TRUE puts a flag for field welding |
| Input: | (VARIANT\_BOOL) showOtherSide | Not used; pass 0 |
| Input: | (VARIANT\_BOOL) dashOnTop | TRUE puts the dash line on top |
| Input: | (VARIANT\_BOOL) peripheral | TRUE puts a peripheral symbol |
| Input: | (VARIANT\_BOOL) hasProcess | TRUEto specify a processValue |
| Input: | (BSTR) processValue | Process value if hasProcess is set to TRUE |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks

The symbol argument specifies the weld symbol name. A list of names
can be found in the text file gtol.sym,
which is located in the SolidWorks default installation folder <installation\_dir>\lang\english.
The currently supported list is:

* BUTT
* BUSQ
* BUSV
* BUSB
* BUSVBR
* BUSBR
* BUSU
* BUSJ
* BACK
* FILL
* PLUG
* SPOT
* SEAM