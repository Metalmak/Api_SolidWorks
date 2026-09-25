<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelationManager~IGetAllowedRelations.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetAllowedRelations Method (ISketchRelationManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchRelationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelationManager.html) : IGetAllowedRelations Method (ISketchRelationManager) |

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

*NumAllowedRelations*
:   Number of relations valid for the specified entities

Gets the types of sketch relations valid for the specified entities.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetAllowedRelations( _    ByVal NumEntities As System.Integer, _    ByRef EntityArray As System.Object, _    ByVal NumAllowedRelations As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchRelationManager Dim NumEntities As System.Integer Dim EntityArray As System.Object Dim NumAllowedRelations As System.Integer Dim value As System.Integer   value = instance.IGetAllowedRelations(NumEntities, EntityArray, NumAllowedRelations) ``` | |

| C# |  |
| --- | --- |
| ``` System.int IGetAllowedRelations(     System.int NumEntities,    ref System.object EntityArray,    System.int NumAllowedRelations ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int IGetAllowedRelations(  &   System.int NumEntities, &   System.Object^% EntityArray, &   System.int NumAllowedRelations ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*NumEntities*
:   Number of entities

*EntityArray*
:   Array of entities

*NumAllowedRelations*
:   Number of relations valid for the specified entities

#### Return Value

* in-process, unmanaged C++: Pointer to an array of sketch relation types valid for the specified entities as defined in swConstraintType\_e

- VBA, VB.NET, C#, and C++/CLI: Not supported

  See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Remarks

Call [ISketchRelationManager::IGetAllowedRelationsCount](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchRelationManager~IGetAllowedRelationsCount.html) before calling this method to get the value for NumEntities.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchRelationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelationManager.html)

[ISketchRelationManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelationManager_members.html)

[ISketchRelationManager::GetAllowedRelations Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelationManager~GetAllowedRelations.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0