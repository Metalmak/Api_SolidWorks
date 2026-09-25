<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchUseEdge3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SketchUseEdge3 Method (ISketchManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : SketchUseEdge3 Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Chain*
:   True to convert an entire chain of sketch entities, false to convert only the selected sketch entities (see **Remarks**)

*InnerLoops*
:   True to convert the inner loops of the selected faces to sketch entities, false to not

Creates sketch entities on a sketch plane by projecting selected edges, loops, faces, curves, and external sketch contours.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SketchUseEdge3( _    ByVal Chain As System.Boolean, _    ByVal InnerLoops As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim Chain As System.Boolean Dim InnerLoops As System.Boolean Dim value As System.Boolean   value = instance.SketchUseEdge3(Chain, InnerLoops) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SketchUseEdge3(     System.bool Chain,    System.bool InnerLoops ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SketchUseEdge3(  &   System.bool Chain, &   System.bool InnerLoops ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Chain*
:   True to convert an entire chain of sketch entities, false to convert only the selected sketch entities (see **Remarks**)

*InnerLoops*
:   True to convert the inner loops of the selected faces to sketch entities, false to not

#### Return Value

True if the sketch entities are created, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::SketchUseEdge3.

# ![](dotnetimages/collapse.gif)Example

[Convert Edges and Inner Loops of Face to Sketch Entities (C#)](Convert_Edges_and_Inner_Loops_of_Face_to_Sketch_Entities_Example_CSharp.htm)

[Convert Edges and Inner Loops of Face to Sketch Entities (VB.NET)](Convert_Edges_and_Inner_Loops_of_Face_to_Sketch_Entities_Example_VBNET.htm)

[Convert Edges and Inner Loops of Face to Sketch Entities (VBA)](Convert_Edges_and_Inner_Loops_of_Face_to_Sketch_Entities_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Specifying true for the Chain argument creates the selected sketch entity and any other sketch entities that belong to the same sketch contour or chain (contiguous geometric entities like sketch edges) on the sketch plane.

To display all sketch relations symbols, set [IModelDocExtension::SetUserPreferenceToggle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SetUserPreferenceToggle.html) swViewSketchRelations to true, which can adversely affect performance. To hide all sketch relation symbols, set IModelDocExtension::SetUserPreferenceToggle swViewSketchRelations to false, which can improve performance and was the default setting prior to SOLIDWORKS 2005.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

[IModelDoc2::SketchOffsetEntities2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SketchOffsetEntities2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0