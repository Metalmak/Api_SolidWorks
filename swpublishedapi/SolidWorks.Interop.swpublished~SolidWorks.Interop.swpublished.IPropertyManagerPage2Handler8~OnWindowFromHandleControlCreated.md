<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler8~OnWindowFromHandleControlCreated.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnWindowFromHandleControlCreated Method (IPropertyManagerPage2Handler8) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IPropertyManagerPage2Handler8 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler8.html) : OnWindowFromHandleControlCreated Method (IPropertyManagerPage2Handler8) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Id*
:   ID of this .NET control

*Status*
:   True if the .NET control is successfully created; false if not

Obsolete. Superseded by [IPropertyManagerPage2Handler9::OnWindowFromHandleControlCreated](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler9~OnWindowFromHandleControlCreated.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function OnWindowFromHandleControlCreated( _    ByVal Id As System.Integer, _    ByVal Status As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler8 Dim Id As System.Integer Dim Status As System.Boolean Dim value As System.Integer   value = instance.OnWindowFromHandleControlCreated(Id, Status) ``` | |

| C# |  |
| --- | --- |
| ``` System.int OnWindowFromHandleControlCreated(     System.int Id,    System.bool Status ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int OnWindowFromHandleControlCreated(  &   System.int Id, &   System.bool Status ) ``` | |

#### Parameters

*Id*
:   ID of this .NET control

*Status*
:   True if the .NET control is successfully created; false if not

#### Return Value

If Status = true, return nothing

If Status = false, return an action as defined in swHandleWindowFromHandleCreationFailure\_e

(see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2Handler8::OnWindowFromHandleControlCreated.

# ![](dotnetimages/collapse.gif)Remarks

If the .NET control is not successfully created (Status = false), the program creating the PropertyManager page should receive notification from this handler. Return one of the following options in swHandleWindowFromHandleCreationFailure\_e:

* swHandleWindowFromHandleCreationFailure\_Cancel. Continue creating the PropertyManager page without the .NET control. This is the default.

  * swHandleWindowFromHandleCreationFailure\_Retry. Try to create the .NET control again. You can call the IPropertyManagerPageWindowFromHandle::SetWindowHandle method to change the .NET control handle to perhaps use another similar control or another version of the control, and then return swHandleWindowFromHandleCreationFailure\_Retry. Avoid an endless loop situation.

    * swHandleWindowFromHandleCreationFailure\_Continue. Cancel creating PropertyManager page. For example, it might be that the PropertyManager page is useless without the control, so the calling add-in might want to quit and handle the situation on its own.

For example if the control is created successfully, then SOLIDWORKS passes Status = true to the add-in, and nothing is returned. If the control fails to be created, SOLIDWORKS passes Status = false to the add-in, and the handler returns swHandleWindowFromHandleCreationFailure\_Continue.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler8 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler8.html)

[IPropertyManagerPage2Handler8 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler8_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0