<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5~GetParentInfo.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| GetParentInfo Method (IEdmCardControl5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCardControl5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5.html) : GetParentInfo Method (IEdmCardControl5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*plParentCtrlID*
:   ID of the parent control; 0 if there is no parent control

*plPageNo*
:   0-based index of the tab control on which this control is located

Gets the parent control of this control.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub GetParentInfo( _    ByRef plParentCtrlID As System.Integer, _    ByRef plPageNo As System.Integer _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void GetParentInfo(     out System.int plParentCtrlID,    out System.int plPageNo ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetParentInfo(  &   [Out] System.int plParentCtrlID, &   [Out] System.int plPageNo ) ``` | |

#### Parameters

*plParentCtrlID*
:   ID of the parent control; 0 if there is no parent control

*plPageNo*
:   0-based index of the tab control on which this control is located

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCardControl6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl6.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: The control does not have a parent.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCardControl5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5.html)

[IEdmCardControl5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional Version 5.2