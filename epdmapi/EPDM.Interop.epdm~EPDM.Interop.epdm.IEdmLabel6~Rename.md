<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmLabel6~Rename.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| Rename Method (IEdmLabel6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmLabel6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmLabel6.html) : Rename Method (IEdmLabel6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*bsName*
:   New name of label

*hParentWnd*
:   Parent window handle; passed to add-ins that have registered the hooks, [EdmCmdData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html).EdmCmd\_PreLabelModify and EdmCmdData.EdmCmd\_PostLabelModify

Renames this label.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub Rename( _    ByVal bsName As System.String, _    ByVal hParentWnd As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void Rename(     System.string bsName,    System.int hParentWnd ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void Rename(  &   System.String^ bsName, &   System.int hParentWnd ) ``` | |

#### Parameters

*bsName*
:   New name of label

*hParentWnd*
:   Parent window handle; passed to add-ins that have registered the hooks, [EdmCmdData](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCmdData.html).EdmCmd\_PreLabelModify and EdmCmdData.EdmCmd\_PostLabelModify

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmLabel6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmLabel6.html)

[IEdmLabel6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmLabel6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2011