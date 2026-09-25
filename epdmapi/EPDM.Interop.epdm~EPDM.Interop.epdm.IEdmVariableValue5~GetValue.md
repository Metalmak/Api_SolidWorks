<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableValue5~GetValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetValue Method (IEdmVariableValue5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmVariableValue5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableValue5.html) : GetValue Method (IEdmVariableValue5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsConfiguration*
:   Name of configuration for which to get the value; "" for folders and file types that do not support multiple configurations

Gets the value of this variable in the specified configuration.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetValue( _    ByVal bsConfiguration As System.String _ ) As System.Object ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetValue(     System.string bsConfiguration ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetValue(  &   System.String^ bsConfiguration ) ``` | |

#### Parameters

*bsConfiguration*
:   Name of configuration for which to get the value; "" for folders and file types that do not support multiple configurations

#### Return Value

Value of the variable

# ![](dotnetimages/collapse.gif)Example

See the [IEdmVariableValue5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableValue5.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

C++ users should use VariantInit and VariantClear to handle the VARIANT struct properly.

[Return codes:](ReturnCodes.htm)

* S\_OK: The method successfully executed.* S\_FALSE: No value exists for the specified configuration.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmVariableValue5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableValue5.html)

[IEdmVariableValue5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableValue5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2