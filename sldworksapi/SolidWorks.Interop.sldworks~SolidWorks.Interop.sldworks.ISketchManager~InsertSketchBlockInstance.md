<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~InsertSketchBlockInstance.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertSketchBlockInstance Method (ISketchManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : InsertSketchBlockInstance Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BlockDef*
:   [Block](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchBlockDefinition.html) for this block instance

*Position*
:   [Position](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html) of this block instance

*Scale*
:   Scale for this block instance

*Angle*
:   Rotation angle for this block instance

Inserts a block instance at the specified location using the block definition.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertSketchBlockInstance( _    ByVal BlockDef As SketchBlockDefinition, _    ByVal Position As MathPoint, _    ByVal Scale As System.Double, _    ByVal Angle As System.Double _ ) As SketchBlockInstance ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim BlockDef As SketchBlockDefinition Dim Position As MathPoint Dim Scale As System.Double Dim Angle As System.Double Dim value As SketchBlockInstance   value = instance.InsertSketchBlockInstance(BlockDef, Position, Scale, Angle) ``` | |

| C# |  |
| --- | --- |
| ``` SketchBlockInstance InsertSketchBlockInstance(     SketchBlockDefinition BlockDef,    MathPoint Position,    System.double Scale,    System.double Angle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` SketchBlockInstance^ InsertSketchBlockInstance(  &   SketchBlockDefinition^ BlockDef, &   MathPoint^ Position, &   System.double Scale, &   System.double Angle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BlockDef*
:   [Block](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchBlockDefinition.html) for this block instance

*Position*
:   [Position](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html) of this block instance

*Scale*
:   Scale for this block instance

*Angle*
:   Rotation angle for this block instance

#### Return Value

[Block instance](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchBlockInstance.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::InsertSketchBlockInstance.

# ![](dotnetimages/collapse.gif)Example

[Create Block Definition and Insert Block Instance (VBA)](Create_Block_Definition_and_Insert_Block_Instance_Example_VB.htm)

[Create Block Definition and Insert Block Instance (C#)](Create_Block_Definition_and_Insert_Block_Instance_Example_CSharp.htm)

[Create Block Definition and Insert Block Instance (VB.NET)](Create_Block_Definition_and_Insert_Block_Instance_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method creates a block definition if the block definition does not exist.

-  or -

If the definition exists, then this method uses that block definition to create the block instance. The name of the block instance is the same as the filename of the block file, without the filename extension.

If the entities of a block are associated with one or more layers and those layers do not already exist in the drawing, then the layers are inserted in the drawing and the associations between the entities of the block and the layers are maintained.

The block instance is inserted on the current drawing layer.

**TIP:** If inserting the same sketch block multiple times, do not create the block definition more than once. Instead, use the same block definition for each call to SketchManager::InsertSketchBlockInstance.

To save a block instance and its definition into a block file (**.sldblk**), use [ISketchBlockDefinition::Save](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchBlockDefinition~Save.html).

This method does not work for drawings opened in view-only mode.

See Block Definitions and Block Instances for details.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0