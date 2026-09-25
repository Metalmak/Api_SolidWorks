<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~MoveOrCopy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MoveOrCopy Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : MoveOrCopy Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Copy*
:   True to copy the sketch entities or annotations, false to not

*NumCopies*
:   Number of copies

*KeepRelations*
:   True to keep sketch relations, false to not

*BaseX*
:   X coordinate of the base point from which to move the sketch entities or annotations

*BaseY*
:   Y coordinate of the base point from which to move the sketch entities or annotations

*BaseZ*
:   Z coordinate of the base point from which to move the sketch entities or annotations

*DestX*
:   X coordinate of the destination point to which to move the sketch entities or annotations

*DestY*
:   Y coordinate of the destination point to which to move the sketch entities or annotations

*DestZ*
:   Z coordinate of the destination point to which to move the sketch entities or annotations

Moves and optionally copies the selected sketch entities or annotations.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub MoveOrCopy( _    ByVal Copy As System.Boolean, _    ByVal NumCopies As System.Integer, _    ByVal KeepRelations As System.Boolean, _    ByVal BaseX As System.Double, _    ByVal BaseY As System.Double, _    ByVal BaseZ As System.Double, _    ByVal DestX As System.Double, _    ByVal DestY As System.Double, _    ByVal DestZ As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Copy As System.Boolean Dim NumCopies As System.Integer Dim KeepRelations As System.Boolean Dim BaseX As System.Double Dim BaseY As System.Double Dim BaseZ As System.Double Dim DestX As System.Double Dim DestY As System.Double Dim DestZ As System.Double   instance.MoveOrCopy(Copy, NumCopies, KeepRelations, BaseX, BaseY, BaseZ, DestX, DestY, DestZ) ``` | |

| C# |  |
| --- | --- |
| ``` void MoveOrCopy(     System.bool Copy,    System.int NumCopies,    System.bool KeepRelations,    System.double BaseX,    System.double BaseY,    System.double BaseZ,    System.double DestX,    System.double DestY,    System.double DestZ ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void MoveOrCopy(  &   System.bool Copy, &   System.int NumCopies, &   System.bool KeepRelations, &   System.double BaseX, &   System.double BaseY, &   System.double BaseZ, &   System.double DestX, &   System.double DestY, &   System.double DestZ ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Copy*
:   True to copy the sketch entities or annotations, false to not

*NumCopies*
:   Number of copies

*KeepRelations*
:   True to keep sketch relations, false to not

*BaseX*
:   X coordinate of the base point from which to move the sketch entities or annotations

*BaseY*
:   Y coordinate of the base point from which to move the sketch entities or annotations

*BaseZ*
:   Z coordinate of the base point from which to move the sketch entities or annotations

*DestX*
:   X coordinate of the destination point to which to move the sketch entities or annotations

*DestY*
:   Y coordinate of the destination point to which to move the sketch entities or annotations

*DestZ*
:   Z coordinate of the destination point to which to move the sketch entities or annotations

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::MoveOrCopy.

# ![](dotnetimages/collapse.gif)Example

[Move Copy Sketch Entities (C#)](Move_Copy_Sketch_Entities_Example_CSharp.htm)

[Move Copy Sketch Entities (VB.NET)](Move_Copy_Sketch_Entities_Example_VBNET.htm)

[Move Copy Sketch Entities (VBA)](Move_Copy_Sketch_Entities_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::RotateOrCopy Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~RotateOrCopy.html)

[IModelDocExtension::ScaleOrCopy Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ScaleOrCopy.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0