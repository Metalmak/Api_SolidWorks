<!-- source: obsoleteapi/PartDocEvents/PartDocEvents__RegenPostNotify.htm -->

# RegenPostNotify - PartDoc Event

This event is obsolete and has been superseded
by PartDoc event RegenPostNotify2.

Description

Post-notifies the user program
when a part document has been rebuilt.

status = RegenPostNotify ( )

|  |  |  |
| --- | --- | --- |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks

You can also use ModelDoc2::GetUpdateStamp
to determine when changes have taken place in this document.