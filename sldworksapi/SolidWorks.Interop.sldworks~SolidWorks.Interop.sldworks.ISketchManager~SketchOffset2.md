<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchOffset2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SketchOffset2 Method (ISketchManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : SketchOffset2 Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Offset*
:   Offset value; negative value offsets the sketch entities in the opposite direction

*BothDirections*
:   True to offset the sketch entities in both directions, false to offset the sketch entities in one direction

*Chain*
:   True to offset the chain of sketch entities, false to offset only the selected sketch entities (see **Remarks**)

*CapEnds*
:   Cap the ends as defined by swSkOffsetCapEndType\_e

*MakeConstruction*
:   Convert original and offset sketch entities to construction sketch entities as defined by swSkOffsetMakeConstructionType\_e

*AddDimensions*
:   True to include the offset distance in the sketch, false to not

Offsets the selected sketch entities.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SketchOffset2( _    ByVal Offset As System.Double, _    ByVal BothDirections As System.Boolean, _    ByVal Chain As System.Boolean, _    ByVal CapEnds As System.Integer, _    ByVal MakeConstruction As System.Integer, _    ByVal AddDimensions As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim Offset As System.Double Dim BothDirections As System.Boolean Dim Chain As System.Boolean Dim CapEnds As System.Integer Dim MakeConstruction As System.Integer Dim AddDimensions As System.Boolean Dim value As System.Boolean   value = instance.SketchOffset2(Offset, BothDirections, Chain, CapEnds, MakeConstruction, AddDimensions) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SketchOffset2(     System.double Offset,    System.bool BothDirections,    System.bool Chain,    System.int CapEnds,    System.int MakeConstruction,    System.bool AddDimensions ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SketchOffset2(  &   System.double Offset, &   System.bool BothDirections, &   System.bool Chain, &   System.int CapEnds, &   System.int MakeConstruction, &   System.bool AddDimensions ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Offset*
:   Offset value; negative value offsets the sketch entities in the opposite direction

*BothDirections*
:   True to offset the sketch entities in both directions, false to offset the sketch entities in one direction

*Chain*
:   True to offset the chain of sketch entities, false to offset only the selected sketch entities (see **Remarks**)

*CapEnds*
:   Cap the ends as defined by swSkOffsetCapEndType\_e

*MakeConstruction*
:   Convert original and offset sketch entities to construction sketch entities as defined by swSkOffsetMakeConstructionType\_e

*AddDimensions*
:   True to include the offset distance in the sketch, false to not

#### Return Value

True if the selected sketch entities are offset, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::SketchOffset2.

# ![](dotnetimages/collapse.gif)Example

[Offset Sketch (C#)](Sketch_Offset_Example_CSharp.htm)

[Offset Sketch (VB.NET)](Sketch_Offset_Example_VBNET.htm)

[Offset Sketch (VBA)](Sketch_Offset_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Specifying true for Chain offsets the selected sketch entities and any other sketch entities that belong to the same contour or chain (contiguous geometric entities like edges).

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

[IModelDoc2::SketchOffsetEntities2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SketchOffsetEntities2.html)

[IModelDoc2::SketchOffsetEdges Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SketchOffsetEdges.html)

[IModelDocExtension::SketchOffsetOnSurface Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SketchOffsetOnSurface.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2016 FCS, Revision Number 24.0