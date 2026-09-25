<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserNotificationDefinition.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IUserNotificationDefinition Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserNotificationDefinition_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IUserNotificationDefinition Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to a user notification of an add-in.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IUserNotificationDefinition ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IUserNotificationDefinition ``` | |

| C# |  |
| --- | --- |
| ``` public interface IUserNotificationDefinition ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IUserNotificationDefinition ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See UserNotificationDefinition.

# ![](dotnetimages/collapse.gif)Example

See the IUserNotificationHandler examples.

# ![](dotnetimages/collapse.gif)Remarks

A user notification is an add-in dialog that:

* Allows an add-in to display a unique message to SOLIDWORKS users.* Is modeless.* May appear within the context of a document open in its own frame or within SOLIDWORKS itself.* Replaces any previously displayed user notification.* Requires an IUserNotificationHandler to handle user notification events.

# ![](dotnetimages/collapse.gif)Accessors

[ISldWorks::DefineUserNotification](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~DefineUserNotification.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[UserNotificationDefinition](SWObjectModel.pdf#UserNotificationDefinition)

# ![](dotnetimages/collapse.gif)See Also

####

[IUserNotificationDefinition Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IUserNotificationDefinition_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[IMessageBarDefinition Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMessageBarDefinition.html)