<!-- source: obsoleteapi/Face/Face__RemoveInnerLoops.htm -->

# Face::RemoveInnerLoops

This
method is obsolete and has been superseded by Face2::RemoveInnerLoops.

Description

This method removes the inner loops on this face.

Syntax (OLE Automation)

retval
= Face.RemoveInnerLoops ( numOfLoops, innerLoopsIn)

|  |  |  |
| --- | --- | --- |
| Input: | (long) numOfLoops | Number of loops to be removed |
| Input: | (VARIANT) innerLoopsIn | VARIANT of type SafeArray of Dispatch pointers to the inner loops to be removed |
| Return: | (LPDISPATCH) retval | Dispatch pointer to the resulting face object |

Syntax (COM)

status = Face->IRemoveInnerLoops
( numOfLoops, innerLoopsIn, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (long) numOfLoops | Number of loops to be removed |
| Input: | (LPLOOP\*) innerLoopsIn | Pointer to an array of the inner loops to be removed |
| Output: | (LPFACE) retval | Pointer to the resulting face object |
| Return: | (HRESULT)status | S\_OK if successful |