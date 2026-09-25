<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DAssemblyDocEvents_RenameItemNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DAssemblyDocEvents\_RenameItemNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DAssemblyDocEvents\_RenameItemNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*EntityType*
:   Type of item to rename as defined in swNotifyEntityType\_e

*oldName*
:   Current item name

*NewName*
:   New item name

Fired when an item is renamed in one of the SOLIDWORKS tree structures, such as the FeatureManager design tree or the ConfigurationManager tree.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DAssemblyDocEvents_RenameItemNotifyEventHandler( _    ByVal EntityType As System.Integer, _    ByVal oldName As System.String, _    ByVal NewName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DAssemblyDocEvents_RenameItemNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_RenameItemNotifyEventHandler(     System.int EntityType,    System.string oldName,    System.string NewName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DAssemblyDocEvents_RenameItemNotifyEventHandler(  &   System.int EntityType, &   System.String^ oldName, &   System.String^ NewName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*EntityType*
:   Type of item to rename as defined in swNotifyEntityType\_e

*oldName*
:   Current item name

*NewName*
:   New item name

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RenameItemNotify Event (AssemblyDoc).

# ![](dotnetimages/collapse.gif)Example

[Add Component and Mate (VBA)](Add_Component_and_Mate_Example_VB.htm)

[Add Component and Mate (VB.NET)](Add_Component_and_Mate_Example_VBNET.htm)

[Add Component and Mate (C#)](Add_Component_and_Mate_Example_CSharp.htm)

[Fire Notifications When Renaming Components (C#)](Fire_Notifications_When_Renaming_Components_Example_CSharp.htm)

[Fire Notifications When Renaming Components (VB.NET)](Fire_Notifications_When_Renaming_Components_Example_VBNET.htm)

[Fire Notifications When Renaming Components (VBA)](Fire_Notifications_When_Renaming_Components_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This event is also fired when [IComponent2::MakeVirtual](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~MakeVirtual.html) is called.

If developing a C++ application, use swAssemblyRenameItemNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus SP1, Revision Number 10.1