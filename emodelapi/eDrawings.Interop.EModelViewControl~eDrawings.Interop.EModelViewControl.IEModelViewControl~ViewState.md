<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~ViewState.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| ViewState Property (IEModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) > [IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html) : ViewState Property (IEModelViewControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*state*
:   View state as defined by [EMVViewState](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.EMVViewState.html)

Gets or sets the view state.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property ViewState( _    ByVal state As EMVViewState _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEModelViewControl Dim state As EMVViewState Dim value As System.Boolean   instance.ViewState(state) = value   value = instance.ViewState(state) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ViewState(     EMVViewState state ) {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool ViewState {    System.bool get(EMVViewState state);    void set (EMVViewState state, System.bool value); } ``` | |

#### Parameters

*state*
:   View state as defined by [EMVViewState](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.EMVViewState.html)

#### Property Value

True if the view state is set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EModelViewControl::ViewState.

# ![](dotnetimages/collapse.gif)Example

MyEModelViewControl.ViewState(eMVPerspective) = True 'Sets view state to perspective or true

MyEModelViewControl.ViewState(eMVPerspective) ' Gets view state

See [IEModelViewControl](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html)

[IEModelViewControl Members](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl_members.html)

[IEModelViewControl::ShowShadedEdges Property ()](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~ShowShadedEdges.html)

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2005 SP0