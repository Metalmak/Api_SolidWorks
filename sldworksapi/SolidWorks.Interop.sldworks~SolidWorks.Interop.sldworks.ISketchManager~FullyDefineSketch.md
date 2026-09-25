<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~FullyDefineSketch.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FullyDefineSketch Method (ISketchManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : FullyDefineSketch Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*EntitiesToFullyDefine*
:   True to fully define all entities, false to fully define only the entities selected

*UseRelations*
:   True to use relations, false to not

*RelationsToApply*
:   Relations to apply as defined in swSketchFullyDefineRelationType\_e

*UseDimensions*
:   True to use dimensions, false to not

*HorizontalDimScheme*
:   * 0 = Chain

    - 1 = Baseline

      - 2 = Ordinate

*HorizontalDatumDisp*
:   Horizontal datum (model edge, model vertex, sketch line, sketch point), or, if Nothing or null, use entity with selection mark = 6

*VerticalDimScheme*
:   * 0 = Chain

    - 1 = Baseline

      - 2 = Ordinate

*VerticalDatumDisp*
:   Vertical datum (model edge, model vertex, sketch line, sketch point), or, if Nothing or null, use entity with selection mark = 6

*HorizontalDimPlacement*
:   * 0 = Above sketch

    - 1 = Below sketch

*VerticalDimPlacement*
:   * 0 = Right of sketch

    - 1 = Left of sketch

Fully defines a sketch.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FullyDefineSketch( _    ByVal EntitiesToFullyDefine As System.Boolean, _    ByVal UseRelations As System.Boolean, _    ByVal RelationsToApply As System.Integer, _    ByVal UseDimensions As System.Boolean, _    ByVal HorizontalDimScheme As System.Integer, _    ByVal HorizontalDatumDisp As System.Object, _    ByVal VerticalDimScheme As System.Integer, _    ByVal VerticalDatumDisp As System.Object, _    ByVal HorizontalDimPlacement As System.Integer, _    ByVal VerticalDimPlacement As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim EntitiesToFullyDefine As System.Boolean Dim UseRelations As System.Boolean Dim RelationsToApply As System.Integer Dim UseDimensions As System.Boolean Dim HorizontalDimScheme As System.Integer Dim HorizontalDatumDisp As System.Object Dim VerticalDimScheme As System.Integer Dim VerticalDatumDisp As System.Object Dim HorizontalDimPlacement As System.Integer Dim VerticalDimPlacement As System.Integer Dim value As System.Integer   value = instance.FullyDefineSketch(EntitiesToFullyDefine, UseRelations, RelationsToApply, UseDimensions, HorizontalDimScheme, HorizontalDatumDisp, VerticalDimScheme, VerticalDatumDisp, HorizontalDimPlacement, VerticalDimPlacement) ``` | |

| C# |  |
| --- | --- |
| ``` System.int FullyDefineSketch(     System.bool EntitiesToFullyDefine,    System.bool UseRelations,    System.int RelationsToApply,    System.bool UseDimensions,    System.int HorizontalDimScheme,    System.object HorizontalDatumDisp,    System.int VerticalDimScheme,    System.object VerticalDatumDisp,    System.int HorizontalDimPlacement,    System.int VerticalDimPlacement ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int FullyDefineSketch(  &   System.bool EntitiesToFullyDefine, &   System.bool UseRelations, &   System.int RelationsToApply, &   System.bool UseDimensions, &   System.int HorizontalDimScheme, &   System.Object^ HorizontalDatumDisp, &   System.int VerticalDimScheme, &   System.Object^ VerticalDatumDisp, &   System.int HorizontalDimPlacement, &   System.int VerticalDimPlacement ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*EntitiesToFullyDefine*
:   True to fully define all entities, false to fully define only the entities selected

*UseRelations*
:   True to use relations, false to not

*RelationsToApply*
:   Relations to apply as defined in swSketchFullyDefineRelationType\_e

*UseDimensions*
:   True to use dimensions, false to not

*HorizontalDimScheme*
:   * 0 = Chain

    - 1 = Baseline

      - 2 = Ordinate

*HorizontalDatumDisp*
:   Horizontal datum (model edge, model vertex, sketch line, sketch point), or, if Nothing or null, use entity with selection mark = 6

*VerticalDimScheme*
:   * 0 = Chain

    - 1 = Baseline

      - 2 = Ordinate

*VerticalDatumDisp*
:   Vertical datum (model edge, model vertex, sketch line, sketch point), or, if Nothing or null, use entity with selection mark = 6

*HorizontalDimPlacement*
:   * 0 = Above sketch

    - 1 = Below sketch

*VerticalDimPlacement*
:   * 0 = Right of sketch

    - 1 = Left of sketch

#### Return Value

Not currently defined

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::FullyDefineSketch.

# ![](dotnetimages/collapse.gif)Example

[Fully Define Under Defined Sketch (VBA)](Fully_Define_Underdefined_Sketch_Example_VB.htm)

[Fully Define Under Defined Sketch (VB.NET)](Fully_Define_Underdefined_Sketch_Example_VBNET.htm)

[Fully Define Under Defined Sketch (C#)](Fully_Define_Underdefined_Sketch_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

[ISketchManager::AddAlongXDimension Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~AddAlongXDimension.html)

[ISketchManager::AddAlongYDimension Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~AddAlongYDimension.html)

[ISketchManager::AddAlongZDimension Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~AddAlongZDimension.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0