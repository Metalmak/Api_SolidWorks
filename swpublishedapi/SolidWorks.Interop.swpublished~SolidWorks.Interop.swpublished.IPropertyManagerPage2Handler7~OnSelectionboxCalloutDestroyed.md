<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler7~OnSelectionboxCalloutDestroyed.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnSelectionboxCalloutDestroyed Method (IPropertyManagerPage2Handler7) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IPropertyManagerPage2Handler7 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler7.html) : OnSelectionboxCalloutDestroyed Method (IPropertyManagerPage2Handler7) |

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

Obsoleted. Superseded by [IPropertyManagerPage2Handler8::OnSelectionboxCalloutDestroyed](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler8~OnSelectionboxCalloutDestroyed.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub OnSelectionboxCalloutDestroyed( _    ByVal Id As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler7 Dim Id As System.Integer   instance.OnSelectionboxCalloutDestroyed(Id) ``` | |

| C# |  |
| --- | --- |
| ``` void OnSelectionboxCalloutDestroyed(     System.int Id ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OnSelectionboxCalloutDestroyed(  &   System.int Id ) ``` | |

#### Parameters

*Id*
:   ID of this selection box

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2Handler7::OnSelectionboxCalloutDestroyed.

# ![](dotnetimages/collapse.gif)Remarks

This method is:

* only called if callouts have been enabled for the selection box as indicated by the Id argument. Use IPropertyManagerPageSelectionbox::SetCalloutLabel to enable callouts.

  * a post-notification. The callout pointed to by IPropertyManagerPageSelectionbox::Callout no longer exists, so do not make any calls to ICallout methods.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler7 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler7.html)

[IPropertyManagerPage2Handler7 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler7_members.html)

[IPropertyManagerPage2Handler7:;OnSelectionboxCalloutCreated Method](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler7~OnSelectionboxCalloutCreated.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0