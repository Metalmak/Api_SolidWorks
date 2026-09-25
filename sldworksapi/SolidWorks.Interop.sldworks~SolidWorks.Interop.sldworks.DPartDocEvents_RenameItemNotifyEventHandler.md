<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DPartDocEvents_RenameItemNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DPartDocEvents\_RenameItemNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DPartDocEvents\_RenameItemNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*EntityType*
:   Type of item renamed as defined in swNotifyEntityType\_e

*oldName*
:   Previous item name

*NewName*
:   New item name

Fired when an item is renamed in one of the SOLIDWORKS tree structures, such as the FeatureManager design tree or the ConfigurationManager.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DPartDocEvents_RenameItemNotifyEventHandler( _    ByVal EntityType As System.Integer, _    ByVal oldName As System.String, _    ByVal NewName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DPartDocEvents_RenameItemNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DPartDocEvents_RenameItemNotifyEventHandler(     System.int EntityType,    System.string oldName,    System.string NewName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DPartDocEvents_RenameItemNotifyEventHandler(  &   System.int EntityType, &   System.String^ oldName, &   System.String^ NewName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*EntityType*
:   Type of item renamed as defined in swNotifyEntityType\_e

*oldName*
:   Previous item name

*NewName*
:   New item name

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RenameItemNotify Event (PartDoc).

# ![](dotnetimages/collapse.gif)Example

[Fire Notifications When Renaming Part Document Belonging to Assembly (C#)](Fire_Notifications_When_Renaming_Part_Document_Belonging_to_Assembly_Example_CSharp.htm)

[Fire Notifications When Renaming Part Document Belonging to Assembly (VB.NET)](Fire_Notifications_When_Renaming_Part_Document_Belonging_to_Assembly_Example_VBNET.htm)

[Fire Notifications When Renaming Part Document Belonging to Assembly (VBA)](Fire_Notifications_When_Renaming_Part_Document_Belonging_to_Assembly_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swPartRenameItemNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus SP1, Revision Number 10.1