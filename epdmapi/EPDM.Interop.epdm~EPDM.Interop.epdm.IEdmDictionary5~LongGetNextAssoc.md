<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~LongGetNextAssoc.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| LongGetNextAssoc Method (IEdmDictionary5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmDictionary5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5.html) : LongGetNextAssoc Method (IEdmDictionary5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the next key-value pair (see **Remarks**)

*plRetKey*
:   Key in the next pair

*pbsRetValue*
:   Value in the next pair

Gets the key-value pair at the next position of an enumeration.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub LongGetNextAssoc( _    ByVal poPos As IEdmPos5, _    ByRef plRetKey As System.Integer, _    ByRef pbsRetValue As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void LongGetNextAssoc(     IEdmPos5 poPos,    out System.int plRetKey,    out System.string pbsRetValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void LongGetNextAssoc(  &   IEdmPos5^ poPos, &   [Out] System.int plRetKey, &   [Out] System.String^ pbsRetValue ) ``` | |

#### Parameters

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the next key-value pair (see **Remarks**)

*plRetKey*
:   Key in the next pair

*pbsRetValue*
:   Value in the next pair

# ![](dotnetimages/collapse.gif)Example

[Get and Set Dictionary Key-Value Pairs (VB.NET)](Get_and_Set_Key_Value_Pairs_Example_VBNET.htm)

[Get and Set Dictionary Key-Value Pairs (C#)](Get_and_Set_Key_Value_Pairs_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method the first time, you must populate poPos with the interface to the position of the first key-value pair. Call one of the following to obtain IEdmPos5 for the position of the first pair:

* [IEdmDictionary5::LongGetFirstPosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~LongGetFirstPosition.html)* [IEdmDictionary5::LongFindKeys](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~LongFindKeys.html)* [IEdmDictionary5::LongFindValues](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~LongFindValues.html)

After calling this method the first time, poPos is automatically incremented every time it is called. Call this method repeatedly to obtain the rest of the key-value pairs.

Between calls, you should call [IEdmPos5::IsNull](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5~IsNull.html) to verify that you have not gone past the last key-value pair.

C++ programmers must release the returned string by calling SysFreeString.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_END\_OF\_LIST: You have gone past the end of the list.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmDictionary5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5.html)

[IEdmDictionary5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5_members.html)

[IEdmDictionary5::StringGetNextAssoc Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~StringGetNextAssoc.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2