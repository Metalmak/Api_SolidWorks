<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelationManager~IGetAllowedRelationsCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetAllowedRelationsCount Method (ISketchRelationManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchRelationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelationManager.html) : IGetAllowedRelationsCount Method (ISketchRelationManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*NumEntities*
:   Number of entities

*EntityArray*
:   Array of entities

Gets the number of sketch relations valid for the specified entities.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetAllowedRelationsCount( _    ByVal NumEntities As System.Integer, _    ByRef EntityArray As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchRelationManager Dim NumEntities As System.Integer Dim EntityArray As System.Object Dim value As System.Integer   value = instance.IGetAllowedRelationsCount(NumEntities, EntityArray) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IGetAllowedRelationsCount(     System.int NumEntities,    ref System.object EntityArray ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IGetAllowedRelationsCount(  &   System.int NumEntities, &   System.Object^% EntityArray ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumEntities*
:   Number of entities

*EntityArray*
:   Array of entities

#### Return Value

Number of sketch relations valid for the specified entities

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchRelationManager::IGetAllowedRelationsCount.

# ![](dotnetimages/collapse.gif)Remarks

Call this method before calling [ISketchRelationManager::IGetAllowedRelations](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchRelationManager~IGetAllowedRelations.html) to get the size of the array for that method.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchRelationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelationManager.html)

[ISketchRelationManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelationManager_members.html)

[ISketchRelationManager::GetAllowedRelations Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelationManager~GetAllowedRelations.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0