<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate~SetVar.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetVar Method (IEdmBatchUpdate) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchUpdate Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate.html) : SetVar Method (IEdmBatchUpdate) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFileID*
:   ID of file to which to write the variable

*lVariableID*
:   ID of variable to update; retrieve using [IEdmVariableMgr5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr5.html)

*poValue*
:   New value of the variable

*bsConfiguration*
:   Name of the configuration to which to write the variable; empty string for files without configurations

*lEdmBatchFlags*
:   Combination of [EdmBatchFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchFlags.html) bits

Obsolete. Superseded by [IEdmBatchUpdate2::SetVar](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2~SetVar.html).

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
:   ID of file to which to write the variable

*lVariableID*
:   ID of variable to update; retrieve using [IEdmVariableMgr5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmVariableMgr5.html)

*poValue*
:   New value of the variable

*bsConfiguration*
:   Name of the configuration to which to write the variable; empty string for files without configurations

*lEdmBatchFlags*
:   Combination of [EdmBatchFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchFlags.html) bits

# ![](dotnetimages/collapse.gif)Remarks

See the [IEdmBatchUpdate](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate.html) remarks for information about using this method.

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchUpdate Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate.html)

[IEdmBatchUpdate Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 6.2