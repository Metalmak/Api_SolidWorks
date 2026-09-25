<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DPartDocEvents_PreRenameItemNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DPartDocEvents\_PreRenameItemNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DPartDocEvents\_PreRenameItemNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*EntityType*
:   :   Type of item to rename as defined in swNotifyEntityType\_e

*oldName*
:   :   Current name of the part document

*NewName*
:   New name of the part document

Fired when a part document referenced by other documents is about to be renamed.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DPartDocEvents_PreRenameItemNotifyEventHandler( _    ByVal EntityType As System.Integer, _    ByVal oldName As System.String, _    ByVal NewName As System.String _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DPartDocEvents_PreRenameItemNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DPartDocEvents_PreRenameItemNotifyEventHandler(     System.int EntityType,    System.string oldName,    System.string NewName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DPartDocEvents_PreRenameItemNotifyEventHandler(  &   System.int EntityType, &   System.String^ oldName, &   System.String^ NewName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*EntityType*
:   :   Type of item to rename as defined in swNotifyEntityType\_e

*oldName*
:   :   Current name of the part document

*NewName*
:   New name of the part document

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PreRenameItemNotify Event (PartDoc).

# ![](dotnetimages/collapse.gif)Example

[Fire Notifications When Renaming Part Document Belonging to Assembly (C#)](Fire_Notifications_When_Renaming_Part_Document_Belonging_to_Assembly_Example_CSharp.htm)

[Fire Notifications When Renaming Part Document Belonging to Assembly (VB.NET)](Fire_Notifications_When_Renaming_Part_Document_Belonging_to_Assembly_Example_VBNET.htm)

[Fire Notifications When Renaming Part Document Belonging to Assembly (VBA)](Fire_Notifications_When_Renaming_Part_Document_Belonging_to_Assembly_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

If developing a C++ application, use swPartPreRenameItemNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0