<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DAssemblyDocEvents_AddItemNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DAssemblyDocEvents\_AddItemNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DAssemblyDocEvents\_AddItemNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*EntityType*
:   Type of item to add as defined in swNotifyEntityType\_e

*itemName*
:   Name of the added item

Notifies the user when a component is added to the FeatureManager design tree.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DAssemblyDocEvents_AddItemNotifyEventHandler( _    ByVal EntityType As System.Integer, _    ByVal itemName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DAssemblyDocEvents_AddItemNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_AddItemNotifyEventHandler(     System.int EntityType,    System.string itemName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_AddItemNotifyEventHandler(  &   System.int EntityType, &   System.String^ itemName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*EntityType*
:   Type of item to add as defined in swNotifyEntityType\_e

*itemName*
:   Name of the added item

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AddItemNotify Event (AssemblyDoc).

# ![](dotnetimages/collapse.gif)Example

[Add Component and Mate (VBA)](Add_Component_and_Mate_Example_VB.htm)

[Add Component and Mate (VB.NET)](Add_Component_and_Mate_Example_VBNET.htm)

[Add Component and Mate (C#)](Add_Component_and_Mate_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

RenameItemNotify is also fired when [IComponent2::MakeVirtual](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~MakeVirtual.html) is called.

If developing a C++ application, use swAssemblyAddItemNotify to register for this notification.

No explicit notification is available for reordering components. However, these actions generate this event and the [DeleteItemNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DAssemblyDocEvents_DeleteItemNotifyEventHandler.html) event.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus SP1, Revision Number 10.1