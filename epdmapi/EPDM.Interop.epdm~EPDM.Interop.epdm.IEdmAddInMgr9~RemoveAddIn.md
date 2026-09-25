<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr9~RemoveAddIn.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| RemoveAddIn Method (IEdmAddInMgr9) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmAddInMgr9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr9.html) : RemoveAddIn Method (IEdmAddInMgr9) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

*oNameOrID*
:   ID or name of the add-in to remove

Removes the specified add-in.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` Sub RemoveAddIn( _    ByVal oNameOrID As System.Object _ ) ``` | |

| C# |  |
| --- | --- |
| ``` void RemoveAddIn(     System.object oNameOrID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void RemoveAddIn(  &   System.Object^ oNameOrID ) ``` | |

#### Parameters

*oNameOrID*
:   ID or name of the add-in to remove

# ![](dotnetimages/collapse.gif)Example

See the [IEdmAddInMgr9](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr9.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

[Return codes](ReturnCodes.htm):

* S\_OK: The method successfully executed.* S\_FALSE: One of the arguments is invalid.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmAddInMgr9 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr9.html)

[IEdmAddInMgr9 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr9_members.html)

[IEdmAddInMgr5::AddAddIns Method ()](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmAddInMgr5~AddAddIns.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2018