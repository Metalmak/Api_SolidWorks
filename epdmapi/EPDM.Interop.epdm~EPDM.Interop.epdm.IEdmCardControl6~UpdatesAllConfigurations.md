<!-- source: epdmapi/EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl6~UpdatesAllConfigurations.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS PDM Professional API Help | Send Feedback |
| UpdatesAllConfigurations Property (IEdmCardControl6) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [EPDM.Interop.epdm Namespace](EPDM.Interop.epdm~EPDM.Interop.epdm_namespace.html) > [IEdmCardControl6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl6.html) : UpdatesAllConfigurations Property (IEdmCardControl6) |

[ ]

Visual Basic

[ ]

C#

[ ]

C++/CLI

Gets whether this edit box control updates all configuration tabs of the file data card.

# ![](dotnetimages/collapse.gif)Syntax

| Visual Basic |  |
| --- | --- |
| ``` ReadOnly Property UpdatesAllConfigurations As System.Boolean ``` | |

| C# |  |
| --- | --- |
| ``` System.bool UpdatesAllConfigurations {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool UpdatesAllConfigurations {    System.bool get(); } ``` | |

#### Property Value

True to update all configuration tabs, false to not

# ![](dotnetimages/collapse.gif)Example

See the [IEdmCardControl6](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl6.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This property:

* corresponds to the **Updates all configurations** check box in the Edit-box properties panel of the Card Editor.* is valid only if [IEdmCardControl5::ControlType](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl5~ControlType.html) is [EdmCardControlType](EPDM.Interop.epdm~EPDM.Interop.epdm.EdmCardControlType.html).EdmCtrl\_Editbox.

# ![](dotnetimages/collapse.gif)See Also

####

[IEdmCardControl6 Interface](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl6.html)

[IEdmCardControl6 Members](EPDM.Interop.epdm~EPDM.Interop.epdm.IEdmCardControl6_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS PDM Professional 2015 SP02