<!-- source: obsoleteapi/ModelDoc2/ModelDoc2__SketchTrim.htm -->

# ModelDoc2::SketchTrim

This method is obsolete and has been superseded
by SketchManager::SketchExtend
and SketchManager::SketchTrim.

Description

This method trims or extends the selected sketch entity.

Syntax (OLE Automation)

void ModelDoc2.SketchTrim ( op, selEnd,
x, y)

| Input: | (long) op | Operation to perform   * 1= Trim * 2 = Extend |
| Input: | (long) selEnd | Not used |
| Input: | (double) x | X pick location |
| Input: | (double) y | Y pick location |

Syntax
(COM)

status = ModelDoc2->SketchTrim (
op, selEnd, x, y )

| Input: | (long) op | Operation to perform   * 1= Trim * 2 = Extend |
| Input: | (long) selEnd | Not used |
| Input: | (double) x | X pick location |
| Input: | (double) y | Y pick location |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks