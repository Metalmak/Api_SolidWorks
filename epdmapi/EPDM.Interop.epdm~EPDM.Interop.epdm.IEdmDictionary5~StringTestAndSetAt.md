<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~StringTestAndSetAt.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| StringTestAndSetAt Method (IEdmDictionary5) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmDictionary5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5.html) : StringTestAndSetAt Method (IEdmDictionary5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsKey*
:   Key for which to set a value

*bsValue*
:   New value

Creates the specified string key if it does not exist and sets its value.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function StringTestAndSetAt( _    ByVal bsKey As System.String, _    ByVal bsValue As System.String _ ) As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool StringTestAndSetAt(     System.string bsKey,    System.string bsValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool StringTestAndSetAt(  &   System.String^ bsKey, &   System.String^ bsValue ) ``` | |

#### Parameters

*bsKey*
:   Key for which to set a value

*bsValue*
:   New value

#### Return Value

True if the value of a new key is successfully set, false if not

# ![](dotnetimages/collapse.gif)Example

[Change Card Variables Add-in (VB.NET)](Change_Card_Variables_Addin_Example_VBNET.htm)

[Change Card Variables Add-in (C#)](Change_Card_Variables_Addin_Example_CSharp.htm)

[Create and Delete Dictionaries (C#)](Create_and_Delete_Dictionaries_Example_CSharp.htm)

[Create and Delete Dictionaries (VB.NET)](Create_and_Delete_Dictionaries_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

The testing and setting are both performed in a single operation. A test-and-set function like this is useful when you need a semaphore to synchronize several clients accessing the same data. See the example in [IEdmDictionary5::LongTestAndSetAt](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~LongTestAndSetAt.html).

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmDictionary5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5.html)

[IEdmDictionary5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5_members.html)

[IEdmDictionary5::StringSetAt Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~StringSetAt.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2