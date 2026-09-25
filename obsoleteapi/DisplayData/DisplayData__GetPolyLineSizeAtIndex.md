<!-- source: obsoleteapi/DisplayData/DisplayData__GetPolyLineSizeAtIndex.htm -->

# DisplayData::GetPolyLineSizeAtIndex

This method is obsolete and has been superseded
by DisplayData::GetPolyLineSizeAtIndex2.

Description

This method gets the number of array elements returned by DisplayData::GetPolylineAtIndex.

Syntax (OLE Automation)

retval = DisplayData.GetPolyLineSizeAtIndex
( index )

| Input: | (long) index | Index of the desired polyline where the index begins at zero |
| Return: | (long) retval | Number array elements returned by GetPolylineAtIndex |

Syntax
(COM)

status = DisplayData->GetPolyLineSizeAtIndex
( index, &retval )

| Input: | (long) index | Index of the desired polyline where the index begins at zero |
| Output: | (long) retval | Number array elements returned by GetPolylineAtIndex |
| Return: | (HRESULT) status | S\_OK if successful |