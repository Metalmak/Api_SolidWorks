<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2~SetFolderVar.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| SetFolderVar Method (IEdmBatchUpdate2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchUpdate2 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchUpdate2.html) : SetFolderVar Method (IEdmBatchUpdate2) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lFolderID*
:   ID of folder to which to write the card variable

*lVariableID*
:   ID of folder card variable to update

*poValue*
:   New value of the folder card variable

*lEdmBatchFlags*
:   Combination of [EdmBatchFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmBatchFlags.html) bits

Adds a folder card variable to the batch of variables to update.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub SetFolderVar( _    ByVal lFolderID As System.Integer, _    ByVal lVariableID As System.Integer, _    ByRef poValue As System.Object, _    Optional ByVal lEdmBatchFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void SetFolderVar(     System.int lFolderID,    System.int lVariableID,    ref System.object poValue,    System.int lEdmBatchFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetFolderVar(  &   System.int lFolderID, &   System.int lVariableID, &   System.Object^% poValue, &   System.int lEdmBatchFlags ) ``` | |

#### Parameters

*lFolderID*
:   ID of folder to which to write the card variable

*lVariableID*
:   ID of folder card variable to update

*poValue*
:   New value of the folder card variable

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