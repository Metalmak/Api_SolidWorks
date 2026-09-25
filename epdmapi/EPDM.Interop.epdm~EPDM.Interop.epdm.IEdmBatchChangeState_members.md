<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IEdmBatchChangeState Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) : IEdmBatchChangeState Interface |

The following tables list the members exposed by [IEdmBatchChangeState](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [Comment](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState~Comment.html) | Comment about this state change or transition revocation to add to the history listing. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AddFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState~AddFile.html) | Adds a file to this batch of files whose states you want to change or whose transitions you want to revoke. |
| ![ Method](dotnetimages/Method.gif) | [ChangeState](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState~ChangeState.html) | Obsolete. Superseded by [IEdmBatchChangeState4::ChangeState2.](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState4~ChangeState2.html) |
| ![ Method](dotnetimages/Method.gif) | [CreateTree](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState~CreateTree.html) | Computes the file reference tree and checks that the specified state transition can be performed for the files added to this batch using [IEdmBatchChangeState::AddFile](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState~AddFile.html). |
| ![ Method](dotnetimages/Method.gif) | [GetFileList](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState~GetFileList.html) | Gets the list of files affected by the state change or transition revocation. |
| ![ Method](dotnetimages/Method.gif) | [SetAux](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState~SetAux.html) | Reserved for future use. |
| ![ Method](dotnetimages/Method.gif) | [ShowDlg](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState~ShowDlg.html) | Shows the change state or revoke transition dialog box. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmBatchChangeState Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmBatchChangeState.html)

[EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html)