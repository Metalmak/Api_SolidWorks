<!-- source: obsoleteapi/AssemblyDoc/AssemblyDoc__InsertDerivedPattern.htm -->

# AssemblyDoc::InsertDerivedPattern

This method is obsolete and has been superseded
by FeatureManager::InsertDerivedPattern.

Description

This method creates a derived component from a selected pattern and
seed components.

Syntax (OLE Automation)

retval = AssemblyDoc.InsertDerivedPattern(
)

| Return: | (VARIANT\_BOOL) retval | TRUE if successful, FALSE if not |

Syntax (COM)

status = AssemblyDoc->InsertDerivedPattern
( )

| Return: | (VARIANT\_BOOL) retval | TRUE if successful, FALSE if not |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks

Use ModelDocExtension::SelectByID to select the
components, which must be ordered:

* seed component
   = selection
  mark 1
* pattern feature
   = selection
  mark 2