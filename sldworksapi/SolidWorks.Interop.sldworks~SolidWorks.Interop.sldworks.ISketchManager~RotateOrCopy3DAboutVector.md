<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~RotateOrCopy3DAboutVector.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| RotateOrCopy3DAboutVector Method (ISketchManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : RotateOrCopy3DAboutVector Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Copy*
:   :   True to copy the 3D sketch entities, false to not

*NumCopies*
:   Number of copies

*KeepRelations*
:   True to keep sketch relations, false to not

*BaseX*
:   X coordinate of the base point from which to rotate the 3D sketch entities

*BaseY*
:   Y coordinate of the base point from which to rotate the 3D sketch entities

*BaseZ*
:   Z coordinate of the base point from which to rotate the 3D sketch entities

*VectorXCoord*
:   X vector component of the axis of rotation, parallel to the base point

*VectorYCoord*
:   Y vector component of the axis of rotation, parallel to the base point

*VectorZCoord*
:   Z vector component of the axis of rotation, parallel to the base point

*AngleAboutVector*
:   :   Angle at which to rotate the sketch entities

Rotates, and optionally copies, the selected 3D sketch entities about the specified vector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RotateOrCopy3DAboutVector( _    ByVal Copy As System.Boolean, _    ByVal NumCopies As System.Integer, _    ByVal KeepRelations As System.Boolean, _    ByVal BaseX As System.Double, _    ByVal BaseY As System.Double, _    ByVal BaseZ As System.Double, _    ByVal VectorXCoord As System.Double, _    ByVal VectorYCoord As System.Double, _    ByVal VectorZCoord As System.Double, _    ByVal AngleAboutVector As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim Copy As System.Boolean Dim NumCopies As System.Integer Dim KeepRelations As System.Boolean Dim BaseX As System.Double Dim BaseY As System.Double Dim BaseZ As System.Double Dim VectorXCoord As System.Double Dim VectorYCoord As System.Double Dim VectorZCoord As System.Double Dim AngleAboutVector As System.Double Dim value As System.Boolean   value = instance.RotateOrCopy3DAboutVector(Copy, NumCopies, KeepRelations, BaseX, BaseY, BaseZ, VectorXCoord, VectorYCoord, VectorZCoord, AngleAboutVector) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool RotateOrCopy3DAboutVector(     System.bool Copy,    System.int NumCopies,    System.bool KeepRelations,    System.double BaseX,    System.double BaseY,    System.double BaseZ,    System.double VectorXCoord,    System.double VectorYCoord,    System.double VectorZCoord,    System.double AngleAboutVector ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool RotateOrCopy3DAboutVector(  &   System.bool Copy, &   System.int NumCopies, &   System.bool KeepRelations, &   System.double BaseX, &   System.double BaseY, &   System.double BaseZ, &   System.double VectorXCoord, &   System.double VectorYCoord, &   System.double VectorZCoord, &   System.double AngleAboutVector ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Copy*
:   :   True to copy the 3D sketch entities, false to not

*NumCopies*
:   Number of copies

*KeepRelations*
:   True to keep sketch relations, false to not

*BaseX*
:   X coordinate of the base point from which to rotate the 3D sketch entities

*BaseY*
:   Y coordinate of the base point from which to rotate the 3D sketch entities

*BaseZ*
:   Z coordinate of the base point from which to rotate the 3D sketch entities

*VectorXCoord*
:   X vector component of the axis of rotation, parallel to the base point

*VectorYCoord*
:   Y vector component of the axis of rotation, parallel to the base point

*VectorZCoord*
:   Z vector component of the axis of rotation, parallel to the base point

*AngleAboutVector*
:   :   Angle at which to rotate the sketch entities

#### Return Value

True if the 3D sketch entities rotated and are optionally copied about the specified vector, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::RotateOrCopy3DAboutVector.

# ![](dotnetimages/collapse.gif)Example

[Rotate and Copy 3D Sketch About Vector (VB.NET)](Rotate_and_Copy_3D_Sketch_About_Vector_Example_VBNET.htm)

[Rotate and Copy 3D Sketch About Vector (VBA)](Rotate_and_Copy_3D_Sketch_About_Vector_Example_VB.htm)

[Rotate and Copy 3D Sketch About Vector (C#)](Rotate_and_Copy_3D_Sketch_About_Vector_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

[IModelDocExtension::RotateOrCopy Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~RotateOrCopy.html)

[ISketchManager::RotateOrCopy3DAboutXYZ Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~RotateOrCopy3DAboutXYZ.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0