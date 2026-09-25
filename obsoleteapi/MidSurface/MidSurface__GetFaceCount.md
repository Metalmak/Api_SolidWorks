<!-- source: obsoleteapi/MidSurface/MidSurface__GetFaceCount.htm -->

# MidSurface::GetFaceCount

This method is obsolete
and has been superseded by MidSurface2::GetFaceCount.

Description

This method gets the total number of faces in the MidSurface feature.
If more than one reference surface exists in the MidSurface feature, then
those faces are included in the total count returned.

Syntax (OLE Automation)

retval = MidSurface.GetFaceCount ()

|  |  |  |
| --- | --- | --- |
| Return: | (long) retval | Face count |

Syntax (COM)

status = MidSurface->GetFaceCount
( &retval )

|  |  |  |
| --- | --- | --- |
| Output: | (long) retval | Face count |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks