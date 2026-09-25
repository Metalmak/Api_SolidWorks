<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState3~AllowAdminToRevoke.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| AllowAdminToRevoke Method (IEdmBatchChangeState3) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmBatchChangeState3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState3.html) : AllowAdminToRevoke Method (IEdmBatchChangeState3) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bAllowAdminToRevoke*
:   True to allow an administrator to revoke state transitions of files, false to not

Sets whether an administrator is allowed to revoke state transitions of files in this batch.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub AllowAdminToRevoke( _    ByVal bAllowAdminToRevoke As System.Boolean _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void AllowAdminToRevoke(     System.bool bAllowAdminToRevoke ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AllowAdminToRevoke(  &   System.bool bAllowAdminToRevoke ) ``` | |

#### Parameters

*bAllowAdminToRevoke*
:   True to allow an administrator to revoke state transitions of files, false to not

# ![](dotnetimages/collapse.gif)Example

See the [IEdmBatchChangeState3](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState3.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchChangeState3 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState3.html)

[IEdmBatchChangeState3 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState3_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2013