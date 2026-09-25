<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateSketchPlane.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateSketchPlane Method (ISketchManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : CreateSketchPlane Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Relation1*
:   Relation as defined in swConstraintType\_e for the first selection to position the 3D sketch plane

*Relation2*
:   Relation as defined in swConstraintType\_e for the second selection to position the 3D sketch plane

*Relation3*
:   Relation as defined in swConstraintType\_e for the third selection to position the 3D sketch plane

Creates a 3D sketch plane.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateSketchPlane( _    ByVal Relation1 As System.Integer, _    ByVal Relation2 As System.Integer, _    ByVal Relation3 As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim Relation1 As System.Integer Dim Relation2 As System.Integer Dim Relation3 As System.Integer Dim value As System.Boolean   value = instance.CreateSketchPlane(Relation1, Relation2, Relation3) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool CreateSketchPlane(     System.int Relation1,    System.int Relation2,    System.int Relation3 ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool CreateSketchPlane(  &   System.int Relation1, &   System.int Relation2, &   System.int Relation3 ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Relation1*
:   Relation as defined in swConstraintType\_e for the first selection to position the 3D sketch plane

*Relation2*
:   Relation as defined in swConstraintType\_e for the second selection to position the 3D sketch plane

*Relation3*
:   Relation as defined in swConstraintType\_e for the third selection to position the 3D sketch plane

#### Return Value

True if the 3D sketch plane is created, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::CreateSketchPlane.

# ![](dotnetimages/collapse.gif)Example

[Create 3D Sketch Plane (C#)](Create_3D_Sketch_Plane_Example_CSharp.htm)

[Create 3D Sketch Plane (VB.NET)](Create_3D_Sketch_Plane_Example_VBNET.htm)

[Create 3D Sketch Plane (VBA)](Create_3D_Sketch_Plane_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method gets the selected items from the selection list in the order in which they were selected and applies the specified relation to them. If fewer than three items were selected, then only the first, or first and second, values are used.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0