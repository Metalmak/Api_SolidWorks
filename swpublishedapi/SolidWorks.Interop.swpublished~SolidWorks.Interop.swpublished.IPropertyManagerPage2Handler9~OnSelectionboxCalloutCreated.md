<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9~OnSelectionboxCalloutCreated.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnSelectionboxCalloutCreated Method (IPropertyManagerPage2Handler9) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IPropertyManagerPage2Handler9 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.html) : OnSelectionboxCalloutCreated Method (IPropertyManagerPage2Handler9) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Id*
:   ID of this selection box

Performs some processing while the callout for this selection box is created.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub OnSelectionboxCalloutCreated( _    ByVal Id As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler9 Dim Id As System.Integer   instance.OnSelectionboxCalloutCreated(Id) ``` | |

| C# |  |
| --- | --- |
| ``` void OnSelectionboxCalloutCreated(     System.int Id ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OnSelectionboxCalloutCreated(  &   System.int Id ) ``` | |

#### Parameters

*Id*
:   ID of this selection box

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2Handler9::OnSelectionboxCalloutCreated.

# ![](dotnetimages/collapse.gif)Example

See the [IPropertyManagerPage2Handler9](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method is only called if callouts have been enabled for the selection box as indicated by the Id argument. Use IPropertyManagerPageSelectionbox::SetCalloutLabel to enable callouts.

You can collect information using this method. For example, you can get the selection type from the last selection. Next, use the IPropertyManagerPageSelectionbox::Callout property to get the ICallout object. Then, use the various ICallout properties to control the callout text and display characteristics based on that selection information.

This method is a pre-notification.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler9 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.html)

[IPropertyManagerPage2Handler9 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9_members.html)

[IPropertyManagerPage2Handler9::OnSelectionboxCalloutDestroyed Method](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9~OnSelectionboxCalloutDestroyed.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 FCS, Revision Number 20.0