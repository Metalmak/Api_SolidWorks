<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9~OnNumberboxChanged.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnNumberboxChanged Method (IPropertyManagerPage2Handler9) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IPropertyManagerPage2Handler9 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.html) : OnNumberboxChanged Method (IPropertyManagerPage2Handler9) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Id*
:   ID of the number box

*Value*
:   Value in the number box

Called when a user changes the value in the number box on a PropertyManager page.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub OnNumberboxChanged( _    ByVal Id As System.Integer, _    ByVal Value As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler9 Dim Id As System.Integer Dim Value As System.Double   instance.OnNumberboxChanged(Id, Value) ``` | |

| C# |  |
| --- | --- |
| ``` void OnNumberboxChanged(     System.int Id,    System.double Value ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OnNumberboxChanged(  &   System.int Id, &   System.double Value ) ``` | |

#### Parameters

*Id*
:   ID of the number box

*Value*
:   Value in the number box

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2Handler9::OnNumberboxChanged.

# ![](dotnetimages/collapse.gif)Example

See the [IPropertyManagerPage2Handler9](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

By default, this method receives a notification every time the value in the number box changes while the slider is being dragged or spun. Numerous notifications result in numerous calls to the handler, which is okay if your application responds quickly to each call. However, if your application responds slowly, then a performance bottleneck might occur.

Set IPropertyManagerPageNumberbox::Style to swPropMgrPageNumberBoxStyle\_e.swPropMgrPageNumberBoxStyle\_SupressNotifyWhileTracking to receive only one notification while the slider is being dragged or spun. [IPropertyManagerPage2Handler9::OnNumberboxTrackingCompleted](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler9~OnNumberBoxTrackingCompleted.html) receives a notification when dragging or spinning of the slider is completed.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler9 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.html)

[IPropertyManagerPage2Handler9 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0