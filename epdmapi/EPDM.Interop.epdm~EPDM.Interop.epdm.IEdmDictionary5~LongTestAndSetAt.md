<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~LongTestAndSetAt.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| LongTestAndSetAt Method (IEdmDictionary5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmDictionary5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5.html) : LongTestAndSetAt Method (IEdmDictionary5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lKey*
:   Key for which to set a value

*bsValue*
:   New value

Creates the specified integer key if it does not exist and sets its value.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function LongTestAndSetAt( _    ByVal lKey As System.Integer, _    ByVal bsValue As System.String _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool LongTestAndSetAt(     System.int lKey,    System.string bsValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool LongTestAndSetAt(  &   System.int lKey, &   System.String^ bsValue ) ``` | |

#### Parameters

*lKey*
:   Key for which to set a value

*bsValue*
:   New value

#### Return Value

True if the value of a new key is successfully set, false otherwise

# ![](dotnetimages/collapse.gif)Example

[Get and Set Dictionary Key-Value Pairs (VB.NET)](Get_and_Set_Key_Value_Pairs_Example_VBNET.htm)

[Get and Set Dictionary Key-Value Pairs (C#)](Get_and_Set_Key_Value_Pairs_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

The testing and the setting are both performed in a single operation. A test-and-set function like this can be useful if you need a semaphore to synchronize several clients accessing the same data.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmDictionary5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5.html)

[IEdmDictionary5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5_members.html)

[IEdmDictionary5::StringTestAndSetAt Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~StringTestAndSetAt.html)

[IEdmDictionary5::LongSetAt Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~LongSetAt.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2