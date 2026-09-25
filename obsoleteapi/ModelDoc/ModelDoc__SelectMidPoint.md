<!-- source: obsoleteapi/ModelDoc/ModelDoc__SelectMidPoint.htm -->

# ModelDoc::SelectMidpoint

This
method is obsolete and has been superseded by ModelDoc2::SelectMidPoint.

Description

When an edge is selected, this method puts the midpoint (swSelMIDPOINTS)
of that edge on the select list and removes the edge from the select list.

Syntax (OLE Automation)

(void) ModelDoc.SelectMidpoint ( )

Syntax (COM)

status = ModelDoc->SelectMidpoint
( )

|  |  |  |
| --- | --- | --- |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

If the edge whose midpoint is desired is already
on the select list and ModelDoc::AndSelect is used to select it again,
then ModelDoc::SelectMidpoint leaves both the edge and the point on the
select list.