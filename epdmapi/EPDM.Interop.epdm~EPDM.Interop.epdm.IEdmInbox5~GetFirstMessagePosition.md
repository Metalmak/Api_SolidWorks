<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmInbox5~GetFirstMessagePosition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFirstMessagePosition Method (IEdmInbox5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmInbox5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmInbox5.html) : GetFirstMessagePosition Method (IEdmInbox5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lEdmGetMsgFlags*
:   Combination of [EdmGetMsgFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetMsgFlag.html) bits indicating which messages to enumerate

Starts an enumeration of the messages in this inbox.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetFirstMessagePosition( _    Optional ByVal lEdmGetMsgFlags As System.Integer _ ) As IEdmPos5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmPos5 GetFirstMessagePosition(     System.int lEdmGetMsgFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmPos5^ GetFirstMessagePosition(  &   System.int lEdmGetMsgFlags ) ``` | |

#### Parameters

*lEdmGetMsgFlags*
:   Combination of [EdmGetMsgFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmGetMsgFlag.html) bits indicating which messages to enumerate

#### Return Value

[IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the first message in the inbox

# ![](dotnetimages/collapse.gif)Example

[Get Messages (C#)](Get_Messages_Example_CSharp.htm)

[Get Messages (VB.NET)](Get_Messages_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method only works to enumerate messages of the user currently logged in to the vault.

After calling this method, pass the returned first message position to [IEdmInbox5::GetNextMessage](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmInbox5~GetNextMessage.html) to get the first message in the inbox. Then call IEdmInbox5::GetNextMessage repeatedly to get the rest of the messages in the inbox.

C++ programmers not using smart-pointer wrapper functions must release the returned interface, IEdmPos5.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_PERMISSION\_DENIED: You tried to access somebody else's messages.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmInbox5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmInbox5.html)

[IEdmInbox5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmInbox5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.3