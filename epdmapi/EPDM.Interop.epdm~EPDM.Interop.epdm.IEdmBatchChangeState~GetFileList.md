<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState~GetFileList.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetFileList Method (IEdmBatchChangeState) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchChangeState Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState.html) : GetFileList Method (IEdmBatchChangeState) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*lEdmChangeStateFileListFlags*
:   Combination of [EdmChangeStateFileListFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmChangeStateFileListFlag.html) bits

Gets the list of files affected by the state change or transition revocation.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Function GetFileList( _    ByVal lEdmChangeStateFileListFlags As System.Integer _ ) As EdmSelectionList5 ``` | |

| C# |  |
| --- | --- |
| ``` EdmSelectionList5 GetFileList(     System.int lEdmChangeStateFileListFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` EdmSelectionList5^ GetFileList(  &   System.int lEdmChangeStateFileListFlags ) ``` | |

#### Parameters

*lEdmChangeStateFileListFlags*
:   Combination of [EdmChangeStateFileListFlag](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmChangeStateFileListFlag.html) bits

#### Return Value

[IEdmSelectionList5](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmSelectionList5.html); list of affected objects

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchChangeState4](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState4.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchChangeState Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState.html)

[IEdmBatchChangeState Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009