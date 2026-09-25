<!-- source: obsoleteapi/DrawingDoc/DrawingDoc__InsertMultiJogLeader2.htm -->

# DrawingDoc::InsertMultiJogLeader2

This method is obsolete and has been superseded
by Drawingdoc::InsertMultiJogLeader3.

Description

This method inserts a multi-jog
leader in this drawing at the specified points.

Syntax (OLE Automation)

lpLeaderDisp = DrawingDoc.InsertMultiJogLeader2 (
points)

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT) points | VARIANT of type SafeArray of points |
| Output: | (LPDISPATCH) lpLeaderDisp | Dispatch pointer to the Leader object |

#

Syntax (COM)

status = DrawingDoc->IInsertMultiJogLeader2 (
pointsCount, points, &lpLeader)

|  |  |  |
| --- | --- | --- |
| Input: | (long) pointsCount | Number of points |
| Property: | (LPMATHPOINT) points | Pointer to the MathPoint object  of size pointsCount |
| Output: | (LPLEADER) lpLeader | Pointer to the Leader object |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks