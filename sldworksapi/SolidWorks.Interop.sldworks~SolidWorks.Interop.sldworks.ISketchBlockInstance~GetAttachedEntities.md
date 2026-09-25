<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance~GetAttachedEntities.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetAttachedEntities Method (ISketchBlockInstance) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchBlockInstance Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance.html) : GetAttachedEntities Method (ISketchBlockInstance) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Entities*
:   Array of attached entities

*EntityTypes*
:   Array of longs or integers (see Long vs. Integer) of the types of attached entities (see **Remarks**)

Gets the entities to which this block instance is attached.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetAttachedEntities( _    ByRef Entities As System.Object, _    ByRef EntityTypes As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchBlockInstance Dim Entities As System.Object Dim EntityTypes As System.Object Dim value As System.Boolean   value = instance.GetAttachedEntities(Entities, EntityTypes) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetAttachedEntities(     out System.object Entities,    out System.object EntityTypes ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetAttachedEntities(  &   [Out] System.Object^ Entities, &   [Out] System.Object^ EntityTypes ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Entities*
:   Array of attached entities

*EntityTypes*
:   Array of longs or integers (see Long vs. Integer) of the types of attached entities (see **Remarks**)

#### Return Value

True if the entities are retrieved, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchBlockInstance::GetAttachedEntities.

# ![](dotnetimages/collapse.gif)Remarks

The arrays returned by this method can contain one or more different object and type.

|  |  |
| --- | --- |
| Possible returned Entities | Possible returned EntityTypes |
| [IFace2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) | swSelFACES |
| [IEdge](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html) | swSelEDGES |
| [IVertex](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IVertex.html) | swSelVERTICES |
| [ISketchSegment](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSegment.html) | swSelSKETCHSEGS |
| [ISketchPoint](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchPoint.html) | swSelSKETCHPOINTS |

A block instance that was inserted with a leader attached to an entity remains attached to that entity even if the leader is hidden. If the leader is shown again later on, the leader still points to the entity and the block instance is still properly associated with the entity.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchBlockInstance Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance.html)

[ISketchBlockInstance Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchBlockInstance_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 SP2, Revision Number 15.2