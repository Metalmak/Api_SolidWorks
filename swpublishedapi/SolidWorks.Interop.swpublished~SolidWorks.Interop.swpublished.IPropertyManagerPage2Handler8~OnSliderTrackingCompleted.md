<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler8~OnSliderTrackingCompleted.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnSliderTrackingCompleted Method (IPropertyManagerPage2Handler8) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IPropertyManagerPage2Handler8 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler8.html) : OnSliderTrackingCompleted Method (IPropertyManagerPage2Handler8) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Id*
:   ID of this slider control

*Value*
:   Value indicating the new position of the slider

Obsolete. Superseded by [IPropertyManagerPage2Handler9::OnSliderTrackingCompleted](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler9~OnSliderTrackingCompleted.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub OnSliderTrackingCompleted( _    ByVal Id As System.Integer, _    ByVal Value As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler8 Dim Id As System.Integer Dim Value As System.Double   instance.OnSliderTrackingCompleted(Id, Value) ``` | |

| C# |  |
| --- | --- |
| ``` void OnSliderTrackingCompleted(     System.int Id,    System.double Value ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OnSliderTrackingCompleted(  &   System.int Id, &   System.double Value ) ``` | |

#### Parameters

*Id*
:   ID of this slider control

*Value*
:   Value indicating the new position of the slider

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2Handler8::OnSliderTrackingCompleted.

# ![](dotnetimages/collapse.gif)Remarks

Although Value is declared as a double, the value of a slider is always a long. When this method is called, Value can be cast to a long.

If IPropertyManagerPageSlider::Style is set to swPropMgrPageSliderStyle\_NotifyWhileTracking, then you can use:

* IPropertyManagerPage2Handler8::OnSliderTrackingCompleted to receive one notification when dragging of the slider is completed.

* [IPropertyManagerPage2Handler8::OnSliderPositionChanged](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler8~OnSliderPositionChanged.html) to receive notifications every time the position of the slider changes because the slider is being dragged.

  NOTE: This might result in numerous calls to the handler, which is fine if the add-in responds quickly to each call. However, if the add-in responds slowly, then a performance bottleneck might occur.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler8 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler8.html)

[IPropertyManagerPage2Handler8 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler8_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0