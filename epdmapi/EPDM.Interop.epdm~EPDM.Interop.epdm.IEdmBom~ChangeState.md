<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom~ChangeState.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| ChangeState Method (IEdmBom) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBom Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom.html) : ChangeState Method (IEdmBom) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*poStateIdOrName*
:   Name or ID of new workflow state

*bsComment*
:   Comment to append to the history of this BOM

*lParentWnd*
:   Parent window handle; passed to registered add-ins

*lEdmStateFlags*
:   Combination of [EdmStateFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmStateFlags.html) bits

Changes the workflow state of this BOM.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub ChangeState( _    ByVal poStateIdOrName As System.Object, _    ByVal bsComment As System.String, _    ByVal lParentWnd As System.Integer, _    Optional ByVal lEdmStateFlags As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void ChangeState(     System.object poStateIdOrName,    System.string bsComment,    System.int lParentWnd,    System.int lEdmStateFlags ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ChangeState(  &   System.Object^ poStateIdOrName, &   System.String^ bsComment, &   System.int lParentWnd, &   System.int lEdmStateFlags ) ``` | |

#### Parameters

*poStateIdOrName*
:   Name or ID of new workflow state

*bsComment*
:   Comment to append to the history of this BOM

*lParentWnd*
:   Parent window handle; passed to registered add-ins

*lEdmStateFlags*
:   Combination of [EdmStateFlags](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmStateFlags.html) bits

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBom Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom.html)

[IEdmBom Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBom_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2009