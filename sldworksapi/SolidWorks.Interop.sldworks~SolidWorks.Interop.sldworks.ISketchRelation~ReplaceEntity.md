<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelation~ReplaceEntity.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ReplaceEntity Method (ISketchRelation) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchRelation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelation.html) : ReplaceEntity Method (ISketchRelation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*OldEntity*
:   Entity to replace

*NewEntity*
:   Replacement entity

Replaces an entity in this sketch relation.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ReplaceEntity( _    ByVal OldEntity As System.Object, _    ByVal NewEntity As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchRelation Dim OldEntity As System.Object Dim NewEntity As System.Object Dim value As System.Boolean   value = instance.ReplaceEntity(OldEntity, NewEntity) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ReplaceEntity(     System.object OldEntity,    System.object NewEntity ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ReplaceEntity(  &   System.Object^ OldEntity, &   System.Object^ NewEntity ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*OldEntity*
:   Entity to replace

*NewEntity*
:   Replacement entity

#### Return Value

True if OldEntity is replaced by NewEntity, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchRelation::ReplaceEntity.

# ![](dotnetimages/collapse.gif)Example

[Replace Sketch Relation (VBA)](Replace_Sketch_Relation_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method requires that the sketch be in edit mode.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchRelation Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelation.html)

[ISketchRelation Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelation_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0