<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~StringSetAt.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| StringSetAt Method (IEdmDictionary5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmDictionary5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5.html) : StringSetAt Method (IEdmDictionary5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsKey*
:   Key whose value to set

*bsValue*
:   New value

Sets the value for the specified string key.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub StringSetAt( _    ByVal bsKey As System.String, _    ByVal bsValue As System.String _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void StringSetAt(     System.string bsKey,    System.string bsValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void StringSetAt(  &   System.String^ bsKey, &   System.String^ bsValue ) ``` | |

#### Parameters

*bsKey*
:   Key whose value to set

*bsValue*
:   New value

# ![](dotnetimages/collapse.gif)Example

See the examples for [IEdmDictionary5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5.html).

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmDictionary5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5.html)

[IEdmDictionary5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5_members.html)

[IEdmDictionary5::StringGetAt Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~StringGetAt.html)

[IEdmDictionary5::StringRemoveAt Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~StringRemoveAt.html)

[IEdmDictionary5::LongSetAt Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmDictionary5~LongSetAt.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2