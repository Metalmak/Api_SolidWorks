<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler5~OnActiveXControlCreated.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnActiveXControlCreated Method (IPropertyManagerPage2Handler5) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IPropertyManagerPage2Handler5 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler5.html) : OnActiveXControlCreated Method (IPropertyManagerPage2Handler5) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Id*
:   ID of this ActiveX control

*Status*
:   True if the ActiveX control creation was successful, false if not

Obsoleted. Superseded by [IPropertyManagerPage2Handler6::OnActiveXControlCreated](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.IPropertyManagerPage2Handler6~OnActiveXControlCreated.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function OnActiveXControlCreated( _    ByVal Id As System.Integer, _    ByVal Status As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPage2Handler5 Dim Id As System.Integer Dim Status As System.Boolean Dim value As System.Integer   value = instance.OnActiveXControlCreated(Id, Status) ``` | |

| C# |  |
| --- | --- |
| ``` System.int OnActiveXControlCreated(     System.int Id,    System.bool Status ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int OnActiveXControlCreated(  &   System.int Id, &   System.bool Status ) ``` | |

#### Parameters

*Id*
:   ID of this ActiveX control

*Status*
:   True if the ActiveX control creation was successful, false if not

#### Return Value

Action to take if the creation of the ActiveX control failed as defined in swHandleActiveXCreationFailure (see Remarks)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPage2Handler5::OnActiveXControlCreated.

# ![](dotnetimages/collapse.gif)Remarks

When the ActiveX control is created, the program creating the PropertyManager page should receive notification from this handler. Specify one of the available enumerators for this handler's retval argument:

* swHandleActiveXCreationFailure\_Cancel. Continue creating the PropertyManager page without the ActiveX control. This is the default.

  * swHandleActiveXCreationFailure\_Retry. Try to create the ActiveX control again. You can reuse the IPropertyManagerPageActiveX::SetClass method to change the control ID or the license key to perhaps use another similar control or another version of the control, and then specify swHandleActiveXCreationFailure\_Retry. Avoid an endless loop situation.

    * swHandleActiveXCreationFailure\_Continue. Cancel creating PropertyManager page. For example, it might be that the PropertyManager page is useless without the control, so the calling add-in might want to quit and handle the situation on its own.

For example, if the control is created successfully, then SOLIDWORKS passes true for Status to the add-in and the return value is ignored. If the control fails to be created, SOLIDWORKS passes false for Status to the add-in and the return value is swHandleActiveXCreationFailure\_Continue.

Do not call IPropertyManagerPageActiveX::GetControl to get the interface object for this ActiveX control.

You cannot get a reference to the ActiveX control inside this event handler because the page is not  displayed when this notification is sent. You can only get the reference to the control after the PropertyManager page is displayed.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPage2Handler5 Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler5.html)

[IPropertyManagerPage2Handler5 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler5_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0