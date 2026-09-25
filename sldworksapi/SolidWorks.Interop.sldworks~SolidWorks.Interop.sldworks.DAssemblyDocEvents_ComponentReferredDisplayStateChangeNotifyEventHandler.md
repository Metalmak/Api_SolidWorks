<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DAssemblyDocEvents_ComponentReferredDisplayStateChangeNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DAssemblyDocEvents\_ComponentReferredDisplayStateChangeNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DAssemblyDocEvents\_ComponentReferredDisplayStateChangeNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*componentModel*
:   [IComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) whose referenced display state is changing

*CompName*
:   Name of component

*oldDSId*
:   Original referenced display state ID of the component

*oldDSName*
:   Original referenced display state name for the component

*newDSId*
:   New referenced display state ID of the component

*newDSName*
:   New referenced display state name for the component

Fired when a component's referenced display state changes.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DAssemblyDocEvents_ComponentReferredDisplayStateChangeNotifyEventHandler( _    ByVal componentModel As System.Object, _    ByVal CompName As System.String, _    ByVal oldDSId As System.Integer, _    ByVal oldDSName As System.String, _    ByVal newDSId As System.Integer, _    ByVal newDSName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DAssemblyDocEvents_ComponentReferredDisplayStateChangeNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_ComponentReferredDisplayStateChangeNotifyEventHandler(     System.object componentModel,    System.string CompName,    System.int oldDSId,    System.string oldDSName,    System.int newDSId,    System.string newDSName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_ComponentReferredDisplayStateChangeNotifyEventHandler(  &   System.Object^ componentModel, &   System.String^ CompName, &   System.int oldDSId, &   System.String^ oldDSName, &   System.int newDSId, &   System.String^ newDSName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*componentModel*
:   [IComponent2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2.html) whose referenced display state is changing

*CompName*
:   Name of component

*oldDSId*
:   Original referenced display state ID of the component

*oldDSName*
:   Original referenced display state name for the component

*newDSId*
:   New referenced display state ID of the component

*newDSName*
:   New referenced display state name for the component

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ComponentReferredDisplayStateChangeNotify Event (AssemblyDoc).

# ![](dotnetimages/collapse.gif)Example

[Fire Notification When Component Referenced Display State Changes (C#)](Fire_Notification_When_Component_Referenced_Display_State_Changes_Example_CSharp.htm)

[Fire Notification When Component Referenced Display State Changes (VB.NET)](Fire_Notification_When_Component_Referenced_Display_State_Changes_Example_VBNET.htm)

[Fire Notification When Component Referenced Display State Changes (VBA)](Fire_Notification_When_Component_Referenced_Display_State_Changed_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use ComponentReferredDisplayStateChangeNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0