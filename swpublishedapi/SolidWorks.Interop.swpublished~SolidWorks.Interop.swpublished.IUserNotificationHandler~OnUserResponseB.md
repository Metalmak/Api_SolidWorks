<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IUserNotificationHandler~OnUserResponseB.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| OnUserResponseB Method (IUserNotificationHandler) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) > [IUserNotificationHandler Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IUserNotificationHandler.html) : OnUserResponseB Method (IUserNotificationHandler) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DoNotShowAgain*
:   True to check "Don't Show Again", false to not

Called by SOLIDWORKS when the user selects the second response control.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub OnUserResponseB( _    ByVal DoNotShowAgain As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IUserNotificationHandler Dim DoNotShowAgain As System.Boolean   instance.OnUserResponseB(DoNotShowAgain) ``` | |

| C# |  |
| --- | --- |
| ``` void OnUserResponseB(     System.bool DoNotShowAgain ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OnUserResponseB(  &   System.bool DoNotShowAgain ) ``` | |

#### Parameters

*DoNotShowAgain*
:   True to check "Don't Show Again", false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See UserNotificationHandler::OnUserResponseB.

# ![](dotnetimages/collapse.gif)Example

See the [IUserNotificationHandler](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IUserNotificationHandler.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IUserNotificationHandler Interface](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IUserNotificationHandler.html)

[IUserNotificationHandler Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.IUserNotificationHandler_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30