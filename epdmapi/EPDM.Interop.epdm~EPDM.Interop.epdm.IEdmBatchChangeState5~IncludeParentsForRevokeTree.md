<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState5~IncludeParentsForRevokeTree.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IncludeParentsForRevokeTree Method (IEdmBatchChangeState5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchChangeState5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState5.html) : IncludeParentsForRevokeTree Method (IEdmBatchChangeState5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bInclude*
:   :   True to include parent files in the file reference tree to revoke transactions, false to not

Gets or sets whether to include parent files in the [file reference tree to revoke transactions](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState2~CreateTreeForRevoke.html).

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub IncludeParentsForRevokeTree( _    ByVal bInclude As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void IncludeParentsForRevokeTree(     System.bool bInclude ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IncludeParentsForRevokeTree(  &   System.bool bInclude ) ``` | |

#### Parameters

*bInclude*
:   :   True to include parent files in the file reference tree to revoke transactions, false to not

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: The argument is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchChangeState5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState5.html)

[IEdmBatchChangeState5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2015 SP04