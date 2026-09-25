<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchOffset.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SketchOffset Method (ISketchManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : SketchOffset Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Offset*
:   Offset value; negative value offsets in opposite direction

*BothDirections*
:   True to offset the sketch entities in both directions, false to not

*Chain*
:   True to offset the chain of sketch entities, false if you want only the selected sketch entities offset (see **Remarks**)

*CapEnds*
:   True to cap the bidirectional offset with arcs, false to not

*MakeConstruction*
:   True to make the sketch entities construction geometry after offsetting, false to not

*AddDimensions*
:   True to include the offset distance in the sketch, false to not

Obsolete. Superseded by [ISketchManager::SketchOffset2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SketchOffset2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SketchOffset( _    ByVal Offset As System.Double, _    ByVal BothDirections As System.Boolean, _    ByVal Chain As System.Boolean, _    ByVal CapEnds As System.Boolean, _    ByVal MakeConstruction As System.Boolean, _    ByVal AddDimensions As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim Offset As System.Double Dim BothDirections As System.Boolean Dim Chain As System.Boolean Dim CapEnds As System.Boolean Dim MakeConstruction As System.Boolean Dim AddDimensions As System.Boolean Dim value As System.Boolean   value = instance.SketchOffset(Offset, BothDirections, Chain, CapEnds, MakeConstruction, AddDimensions) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SketchOffset(     System.double Offset,    System.bool BothDirections,    System.bool Chain,    System.bool CapEnds,    System.bool MakeConstruction,    System.bool AddDimensions ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SketchOffset(  &   System.double Offset, &   System.bool BothDirections, &   System.bool Chain, &   System.bool CapEnds, &   System.bool MakeConstruction, &   System.bool AddDimensions ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Offset*
:   Offset value; negative value offsets in opposite direction

*BothDirections*
:   True to offset the sketch entities in both directions, false to not

*Chain*
:   True to offset the chain of sketch entities, false if you want only the selected sketch entities offset (see **Remarks**)

*CapEnds*
:   True to cap the bidirectional offset with arcs, false to not

*MakeConstruction*
:   True to make the sketch entities construction geometry after offsetting, false to not

*AddDimensions*
:   True to include the offset distance in the sketch, false to not

#### Return Value

True if the sketch entities are offset, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::SketchOffset.

# ![](dotnetimages/collapse.gif)Remarks

Specifying true to the Chain argument offsets the selected entity and any other entities that belong to the same contour or chain (contiguous geometric entities like edges).

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0