<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelationManager~GetRelations.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetRelations Method (ISketchRelationManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchRelationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelationManager.html) : GetRelations Method (ISketchRelationManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Filter*
:   Sketch relation as defined in swSketchRelationFilterType\_e

Gets all of the sketch relations in the sketch based on the specified filter.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetRelations( _    ByVal Filter As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchRelationManager Dim Filter As System.Integer Dim value As System.Object   value = instance.GetRelations(Filter) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetRelations(     System.int Filter ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetRelations(  &   System.int Filter ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Filter*
:   Sketch relation as defined in swSketchRelationFilterType\_e

#### Return Value

Array of [sketch relations](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchRelation.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchRelationManager::GetRelations.

# ![](dotnetimages/collapse.gif)Example

[Replace Sketch Relation (VBA)](Replace_Sketch_Relation_Example_VB.htm)

[Get Sketch Relations (VBA)](Get_Sketch_Relations_Example_VB.htm)

[Get Sketch Relations (VB.NET)](Get_Sketch_Relations_Example_VBNET.htm)

[Get Sketch Relations (C#)](Get_Sketch_Relations_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Because some of the objects may be NULL, you should check for this before accessing them. You should deallocate on any dynamically allocated memory.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchRelationManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelationManager.html)

[ISketchRelationManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelationManager_members.html)

[ISketchRelationManager::IGetRelations Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelationManager~IGetRelations.html)

[ISketchRelationManager::GetRelationsCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelationManager~GetRelationsCount.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0