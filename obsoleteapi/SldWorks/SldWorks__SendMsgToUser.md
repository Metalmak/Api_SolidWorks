<!-- source: obsoleteapi/SldWorks/SldWorks__SendMsgToUser.htm -->

# SldWorks::SendMsgToUser

This method is obsolete and has been superseded
by SldWorks::SendMsgToUser2.

Description

This method displays a message box to the user, who is required to click
on OK to continue.

Syntax (OLE Automation)

void SldWorks.SendMsgToUser ( Message)

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) Message | Message for user |

Syntax (COM)

status = SldWorks->SendMsgToUser
( Message )

|  |  |  |
| --- | --- | --- |
| Input: | (BSTR) Message | Message for user |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks