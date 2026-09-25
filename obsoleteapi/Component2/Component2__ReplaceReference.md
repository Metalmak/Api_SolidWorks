<!-- source: obsoleteapi/Component2/Component2__ReplaceReference.htm -->

# Component2::ReplaceReference

This method is obsolete and has been superseded
by AssemblyDoc::ReplaceComponents.

Description

This method replaces the file name reference
for this component.

Syntax (OLE Automation)

retval = Component2.ReplaceReference ( fileName )

| Input: | (BSTR) fileName | Fully qualified file name, including the path |
| Output: | (long) retval | Error code as defined in swReplaceComponentError\_e |

Syntax (COM)

status = Component2->ReplaceReference ( fileName,
&retval )

| Input: | (BSTR) fileName | Fully qualified file name, including the path |
| Output: | (long) retval | Error code as defined in swReplaceComponentError\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Your application must perform a rebuild after calling
this method.

The component must be a top-level component. It
cannot be a component from a sub-assembly. If the application needs to
replace a component of the sub-assembly, then it should open the sub-assembly
and get the component from that assembly.