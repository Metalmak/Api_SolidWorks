<!-- source: obsoleteapi/AssemblyDoc/AssemblyDoc__IComponentReload3.htm -->

# AssemblyDoc::IComponentReload3

This method is obsolete and has been superseded
by AssemblyDoc::ReplaceComponents.

Description

This method reloads the selected or supplied
component.

Syntax (OLE Automation)

Not available.

Syntax (COM)

status = AssemblyDoc->IComponentReload3 ( component,
readOnly, options, &result )

|  |  |  |
| --- | --- | --- |
| Input: | (LPCOMPONENT) component | Pointer to component to reload |
| Input: | (VARIANT\_BOOL) readOnly | TRUE if the component is to be loaded read-only |
| Input: | (long)options | Control options as defined in swComponentReloadOption\_e |
| Output: | (long)result | Return code as defined in swComponentReloadError\_e |
| Return: | (HRESULT)status | S\_OK if Successful |

Remarks

If the component argument
is set to NULL, then SolidWorks uses the last component in the current
selections.