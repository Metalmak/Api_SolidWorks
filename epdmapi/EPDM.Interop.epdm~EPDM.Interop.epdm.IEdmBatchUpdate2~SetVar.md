<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2~SetVar.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetVar Method (IEdmBatchUpdate2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchUpdate2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2.html) : SetVar Method (IEdmBatchUpdate2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFileID*
:   ID of file to which to write the file card variable

*lVariableID*
:   ID of file card variable to update

*poValue*
:   New value of the file card variable

*bsConfiguration*
:   Name of configuration to which to write the file card variable; ignored if lEdmBatchFlags contains EdmBatchFlags.EdmBatch\_AllConfigs

*lEdmBatchFlags*
:   Combination of [EdmBatchFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchFlags.html) bits

Adds a file card variable to the batch of variables to update.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetVar( _    ByVal lFileID As System.Integer, _    ByVal lVariableID As System.Integer, _    ByRef poValue As System.Object, _    ByVal bsConfiguration As System.String, _    Optional ByVal lEdmBatchFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetVar(     System.int lFileID,    System.int lVariableID,    ref System.object poValue,    System.string bsConfiguration,    System.int lEdmBatchFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetVar(  &   System.int lFileID, &   System.int lVariableID, &   System.Object^% poValue, &   System.String^ bsConfiguration, &   System.int lEdmBatchFlags ) ``` | |

#### Parameters

*lFileID*
:   ID of file to which to write the file card variable

*lVariableID*
:   ID of file card variable to update

*poValue*
:   New value of the file card variable

*bsConfiguration*
:   Name of configuration to which to write the file card variable; ignored if lEdmBatchFlags contains EdmBatchFlags.EdmBatch\_AllConfigs

*lEdmBatchFlags*
:   Combination of [EdmBatchFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchFlags.html) bits

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchUpdate2](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchUpdate2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2.html)

[IEdmBatchUpdate2 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.3