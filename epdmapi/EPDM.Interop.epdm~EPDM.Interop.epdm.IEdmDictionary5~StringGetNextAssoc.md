<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~StringGetNextAssoc.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| StringGetNextAssoc Method (IEdmDictionary5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmDictionary5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5.html) : StringGetNextAssoc Method (IEdmDictionary5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the next key-value pair (see **Remarks**)

*pbsRetKey*
:   Key in the next pair

*pbsRetValue*
:   Value in the next pair

Gets the key-value pair at the next position of an enumeration.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub StringGetNextAssoc( _    ByVal poPos As IEdmPos5, _    ByRef pbsRetKey As System.String, _    ByRef pbsRetValue As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void StringGetNextAssoc(     IEdmPos5 poPos,    out System.string pbsRetKey,    out System.string pbsRetValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void StringGetNextAssoc(  &   IEdmPos5^ poPos, &   [Out] System.String^ pbsRetKey, &   [Out] System.String^ pbsRetValue ) ``` | |

#### Parameters

*poPos*
:   [IEdmPos5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5.html); position of the next key-value pair (see **Remarks**)

*pbsRetKey*
:   Key in the next pair

*pbsRetValue*
:   Value in the next pair

# ![](dotnetimages/collapse.gif)Example

[Change Card Variables Add-in (VB.NET)](Change_Card_Variables_Addin_Example_VBNET.htm)

[Change Card Variables Add-in (C#)](Change_Card_Variables_Addin_Example_CSharp.htm)

[Create and Delete Dictionaries (C#)](Create_and_Delete_Dictionaries_Example_CSharp.htm)

[Create and Delete Dictionaries (VB.NET)](Create_and_Delete_Dictionaries_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method the first time, you must populate poPos with the interface to the position of the first key-value pair. Call one of the following to obtain IEdmPos5 for the position of the first pair:

* [IEdmDictionary5::StringGetFirstPosition](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~StringGetFirstPosition.html)* [IEdmDictionary5::StringFindKeys](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~StringFindKeys.html)* [IEdmDictionary5::StringFindValues](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~StringFindValues.html)

After calling this method the first time, poPos is automatically incremented every time it is called. Call this method repeatedly to obtain the rest of the key-value pairs.

Between calls, you should call [IEdmPos5::IsNull](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmPos5~IsNull.html) to verify that you have not gone past the last key-value pair.

C++ programmers must release the returned strings by calling SysFreeString.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* E\_EDM\_END\_OF\_LIST: You have gone past the end of the list.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmDictionary5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5.html)

[IEdmDictionary5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5_members.html)

[IEdmDictionary5::LongGetNextAssoc Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~LongGetNextAssoc.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2