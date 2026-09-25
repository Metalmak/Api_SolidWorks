<!-- source: obsoleteapi/Sketch/Sketch__GetSplineParamsCount.htm -->

# Sketch::GetSplineParamsCount

This method is obsolete
and is superseded by Sketch::GetSplineParamsCount2.

Description

This method returns the number of splines in the sketch
and the size of array required to hold the data for them.

Syntax (OLE Automation)

Not available.

Syntax (COM)

status = Sketch->GetSplineParamsCount
( &Size, retval )

|  |  |  |
| --- | --- | --- |
| Output: | (long)Size | Size of array required to for a call to Sketch::GetSplineParams |
| Output: | (long)retval | Number of splines |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks