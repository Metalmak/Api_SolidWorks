<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~LongRemoveAt.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| LongRemoveAt Method (IEdmDictionary5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmDictionary5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5.html) : LongRemoveAt Method (IEdmDictionary5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lKey*
:   Key to delete

Deletes the specified integer key and its value.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub LongRemoveAt( _    ByVal lKey As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void LongRemoveAt(     System.int lKey ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void LongRemoveAt(  &   System.int lKey ) ``` | |

#### Parameters

*lKey*
:   Key to delete

# ![](dotnetimages/collapse.gif)Example

[Get and Set Dictionary Key-Value Pairs (VB.NET)](Get_and_Set_Key_Value_Pairs_Example_VBNET.htm)

[Get and Set Dictionary Key-Value Pairs (C#)](Get_and_Set_Key_Value_Pairs_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmDictionary5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5.html)

[IEdmDictionary5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5_members.html)

[IEdmDictionary5::LongSetAt Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~LongSetAt.html)

[IEdmDictionary5::StringRemoveAt Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~StringRemoveAt.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2