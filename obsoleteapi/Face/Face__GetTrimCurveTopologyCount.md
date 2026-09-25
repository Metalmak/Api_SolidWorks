<!-- source: obsoleteapi/Face/Face__GetTrimCurveTopologyCount.htm -->

# Face::GetTrimCurveTopologyCount

This
method is obsolete and has been superseded by Face2::GetTrimCurveTopologyCount.

Description

This method gets the trim curve topology count for this face.

Syntax (OLE Automation)

topologyCount
= Face.GetTrimCurveTopologyCount ( )

|  |  |  |
| --- | --- | --- |
| Return: | (long) topologyCount | Number of elements returned by GetTrimCurveTopology |

Syntax (COM)

status = Face->GetTrimCurveTopologyCount
( &topologyCount )

|  |  |  |
| --- | --- | --- |
| Output: | (long) topologyCount | Number of elements returned by [GetTrimCurveTopology](Face__GetTrimCurveTopology.htm) |
| Return: | (HRESULT) status | S\_OK if successful |