<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~ScaleOrCopy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ScaleOrCopy Method (IModelDocExtension) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : ScaleOrCopy Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Copy*
:   True to copy the sketch items or annotations, false to not

*NumCopies*
:   Number of copies

*BaseX*
:   X coordinate of the base point

*BaseY*
:   Y coordinate of the base point

*BaseZ*
:   Z coordinate of the base point

*Scale*
:   Factor by which to scale the sketch entities or annotations

Scales and optionally copies the selected sketch items or annotations.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ScaleOrCopy( _    ByVal Copy As System.Boolean, _    ByVal NumCopies As System.Integer, _    ByVal BaseX As System.Double, _    ByVal BaseY As System.Double, _    ByVal BaseZ As System.Double, _    ByVal Scale As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim Copy As System.Boolean Dim NumCopies As System.Integer Dim BaseX As System.Double Dim BaseY As System.Double Dim BaseZ As System.Double Dim Scale As System.Double   instance.ScaleOrCopy(Copy, NumCopies, BaseX, BaseY, BaseZ, Scale) ``` | |

| C# |  |
| --- | --- |
| ``` void ScaleOrCopy(     System.bool Copy,    System.int NumCopies,    System.double BaseX,    System.double BaseY,    System.double BaseZ,    System.double Scale ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ScaleOrCopy(  &   System.bool Copy, &   System.int NumCopies, &   System.double BaseX, &   System.double BaseY, &   System.double BaseZ, &   System.double Scale ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Copy*
:   True to copy the sketch items or annotations, false to not

*NumCopies*
:   Number of copies

*BaseX*
:   X coordinate of the base point

*BaseY*
:   Y coordinate of the base point

*BaseZ*
:   Z coordinate of the base point

*Scale*
:   Factor by which to scale the sketch entities or annotations

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::ScaleOrCopy.

# ![](dotnetimages/collapse.gif)Example

[Rotate, Scale, and Copy Sketch (C#)](Rotate_Scale_Copy_Sketch_Example_CSharp.htm)

[Rotate, Scale, and Copy Sketch (VB.NET)](Rotate_Scale_Copy_Sketch_Example_VBNET.htm)

[Rotate, Scale, and Copy Sketch (VBA)](Rotate_Scale_Copy_Sketch_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, use [IModelDocExtension::SelectByID2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByID2.html) to select the entities to scale or copy.

Using this method may break existing sketch relations, including relations that are automatically created when offsetting or converting entities. Use the [ISketchRelationManager](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchRelationManager.html) methods before and after using this method to determine whether all sketch relations remain intact.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::MoveOrCopy Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~MoveOrCopy.html)

[IModelDocExtension::RotateOrCopy Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~RotateOrCopy.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0