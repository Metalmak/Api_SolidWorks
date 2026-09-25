<!-- source: obsoleteapi/Modeler/Modeler__ICheckInterferenceCount.htm -->

# Modeler::ICheckInterferenceCount

This
method is obsolete and has been superceded by Modeler::ICheckInterferenceCount2.

Description

This method checks interference between two
temporary bodies and returns the number of interferences.

Syntax (OLE Automation)

Not available.

Syntax (COM)

status = Modeler->ICheckInterferenceCount ( body1,
body2, coincidentInterference, \*body1InterferedFaceCount, \*body2InterferedFaceCount,
\*intersectedBodyCount, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (LPBODY) body1 | Pointer to a body object to check for interference. |
| Input: | (LPBODY) body2 | Pointer to another body object to check for interference |
| Input: | (VARIANT\_BOOL) coincidentInterference | TRUE to check for coincident interference, FALSE otherwise |
| Output: | (long) \*body1InterferedFaceCount | Number of faces that are interfering that belong to the body passed in the first parameter of this method |
| Output: | (long) \*body2InterferedFaceCount | Number of faces that are interfering that belong to the body passed in the second parameter of this method |
| Output: | (long) \*intersectedBodyCount | Number of intersection bodies produced from this intersection |
| Output: | (VARIANT\_BOOL) retval | TRUE if successful, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Call Modeler::ICheckInterference after calling
this method.