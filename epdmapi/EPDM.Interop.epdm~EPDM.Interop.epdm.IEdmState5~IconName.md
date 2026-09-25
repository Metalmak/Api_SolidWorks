<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5~IconName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| IconName Property (IEdmState5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmState5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5.html) : IconName Property (IEdmState5) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets the name of the icon used in the workflow graph.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` ReadOnly Property IconName As System.String ``` | |

| C# |  |
| --- | --- |
| ``` System.string IconName {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ IconName {    System.String^ get(); } ``` | |

#### Property Value

Name of the icon

# ![](dotnetimages/collapse.gif)Remarks

You can extract the icon from the **WfIcons.dll**, where the resource ID is the name stored in this property appended by "\_SML".

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmState5 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5.html)

[IEdmState5 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmState5_members.html)