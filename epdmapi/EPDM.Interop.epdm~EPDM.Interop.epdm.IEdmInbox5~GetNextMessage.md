<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmInbox5~GetNextMessage.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetNextMessage Method (IEdmInbox5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmInbox5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmInbox5.html) : GetNextMessage Method (IEdmInbox5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the next message (see **Remarks**)

Gets the next message in the enumeration.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetNextMessage( _    ByVal poPos As IEdmPos5 _ ) As IEdmMessage5 ``` | |

| C# |  |
| --- | --- |
| ``` IEdmMessage5 GetNextMessage(     IEdmPos5 poPos ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` IEdmMessage5^ GetNextMessage(  &   IEdmPos5^ poPos ) ``` | |

#### Parameters

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the next message (see **Remarks**)

#### Return Value

[IEdmMessage5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmMessage5.html)

# ![](dotnetimages/collapse.gif)Example

[Get Messages (C#)](Get_Messages_Example_CSharp.htm)

[Get Messages (VB.NET)](Get_Messages_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method the first time, you must populate poPos with the interface to the position of the first message, IEdmPos5. Call [IEdmInbox5::GetFirstMessagePosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmInbox5~GetFirstMessagePosition.html) to obtain IEdmPos5.

After calling this method the first time, poPos is automatically incremented every time it is called. Call this method repeatedly to obtain the rest of the messages.

Be sure to call [IEdmPos5::IsNull](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5~IsNull.html) before you call this method to ensure you have not reached the end of the enumeration.

C++ programmers not using smart-pointer wrapper functions must release the returned interface, IEdmMessage5.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_END\_OF\_LIST: You have gone past the end of the list.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmInbox5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmInbox5.html)

[IEdmInbox5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmInbox5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.3