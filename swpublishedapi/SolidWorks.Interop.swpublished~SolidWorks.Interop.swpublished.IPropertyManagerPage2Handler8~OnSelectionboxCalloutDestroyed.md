<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler8~OnSelectionboxCalloutDestroyed.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnSelectionboxCalloutDestroyed Method (IPropertyManagerPage2Handler8) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IPropertyManagerPage2Handler8 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler8.html) : OnSelectionboxCalloutDestroyed Method (IPropertyManagerPage2Handler8) |

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

Obsolete. Superseded by [IPropertyManagerPage2Handler9::OnSelectionboxCalloutDestroyed](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler9~OnSelectionboxCalloutDestroyed.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub OnSelectionboxCalloutDestroyed( _    ByVal Id As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler8 Dim Id As System.Integer   instance.OnSelectionboxCalloutDestroyed(Id) ``` | |

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

See PropertyManagerPage2Handler8::OnSelectionboxCalloutDestroyed.

# ![](dotnetimages/collapse.gif)Remarks

This method is:

* only called if callouts have been enabled for the selection box as indicated by the Id argument. Use IPropertyManagerPageSelectionbox::SetCalloutLabel to enable callouts.

  * a post-notification. The callout pointed to by IPropertyManagerPageSelectionbox::Callout no longer exists, so do not make any calls to ICallout methods.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler8 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler8.html)

[IPropertyManagerPage2Handler8 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler8_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0