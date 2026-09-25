<!-- source: obsoleteapi/DrawingDoc/DrawingDoc__AddHoleCallout.htm -->

# DrawingDoc::AddHoleCallout

This
method is obsolete and has been superseded by DrawingDoc::AddHoleCallout2.

Description

This method creates a hole callout for the hole as specified by the
selected edge.

Syntax (OLE Automation)

(void)
DrawingDoc.AddHoleCallout ( )

Syntax (COM)

status
= DrawingDoc->AddHoleCallout ( )

|  |  |  |
| --- | --- | --- |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks

This method requires the user to click OK
in the dialog that shows the system-generated hole callout.