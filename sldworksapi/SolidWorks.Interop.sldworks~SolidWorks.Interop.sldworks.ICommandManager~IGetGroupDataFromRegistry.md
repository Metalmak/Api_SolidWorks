<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~IGetGroupDataFromRegistry.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetGroupDataFromRegistry Method (ICommandManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICommandManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager.html) : IGetGroupDataFromRegistry Method (ICommandManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*UserGroupId*
:   User-defined ID of a command group

*Count*
:   Number of command IDs in the given command group

*UserIDs*
:   * in-process, unmanaged C++: Pointer to an array of integer IDs

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

Gets the command IDs of the given command group from the registry.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetGroupDataFromRegistry( _    ByVal UserGroupId As System.Integer, _    ByVal Count As System.Integer, _    ByRef UserIDs As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICommandManager Dim UserGroupId As System.Integer Dim Count As System.Integer Dim UserIDs As System.Integer Dim value As System.Boolean   value = instance.IGetGroupDataFromRegistry(UserGroupId, Count, UserIDs) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IGetGroupDataFromRegistry(     System.int UserGroupId,    System.int Count,    out System.int UserIDs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IGetGroupDataFromRegistry(  &   System.int UserGroupId, &   System.int Count, &   [Out] System.int UserIDs ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*UserGroupId*
:   User-defined ID of a command group

*Count*
:   Number of command IDs in the given command group

*UserIDs*
:   * in-process, unmanaged C++: Pointer to an array of integer IDs

    - VBA, VB.NET, C#, and C++/CLI: Not supported

      See In-process Methods for details about this type of method.

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method call [ICommandManager::GetCommandIDsCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommandManager~GetCommandIDsCount.html) to populate Count.

Use this method to compare command group IDs obtained through the user interface with those stored in the registry.

# ![](dotnetimages/collapse.gif)See Also

####

[ICommandManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager.html)

[ICommandManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager_members.html)

[ICommandManager::GetGroupDataFromRegistry Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandManager~GetGroupDataFromRegistry.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0