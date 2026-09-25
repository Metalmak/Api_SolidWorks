<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~CreateSketchSlot.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| CreateSketchSlot Method (ISketchManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : CreateSketchSlot Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SlotCreationType*
:   Type of sketch slot as defined in swSketchSlotCreationType\_e

*SlotLengthType*
:   Type of length of sketch slot as defined in swSketchSlotLengthType\_e

*Width*
:   Width of sketch slot

*X1*
:   x coordinate of point 1

*Y1*
:   y coordinate of point 1

*Z1*
:   z coordinate of point 2

*X2*
:   x coordinate of point 2

*Y2*
:   y coordinate of point 2

*Z2*
:   z coordinate of point 2

*X3*
:   x coordinate of point 3

*Y3*
:   y coordinate of point 3

*Z3*
:   z coordinate of point 3

*CenterArcDirection*
:   * -1 = Clockwise (CW)* 1 = Counterclockwise (CCW)

*AddDimension*
:   True to automatically add dimensions, false to not

Creates a sketch slot.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateSketchSlot( _    ByVal SlotCreationType As System.Integer, _    ByVal SlotLengthType As System.Integer, _    ByVal Width As System.Double, _    ByVal X1 As System.Double, _    ByVal Y1 As System.Double, _    ByVal Z1 As System.Double, _    ByVal X2 As System.Double, _    ByVal Y2 As System.Double, _    ByVal Z2 As System.Double, _    ByVal X3 As System.Double, _    ByVal Y3 As System.Double, _    ByVal Z3 As System.Double, _    ByVal CenterArcDirection As System.Integer, _    ByVal AddDimension As System.Boolean _ ) As SketchSlot ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim SlotCreationType As System.Integer Dim SlotLengthType As System.Integer Dim Width As System.Double Dim X1 As System.Double Dim Y1 As System.Double Dim Z1 As System.Double Dim X2 As System.Double Dim Y2 As System.Double Dim Z2 As System.Double Dim X3 As System.Double Dim Y3 As System.Double Dim Z3 As System.Double Dim CenterArcDirection As System.Integer Dim AddDimension As System.Boolean Dim value As SketchSlot   value = instance.CreateSketchSlot(SlotCreationType, SlotLengthType, Width, X1, Y1, Z1, X2, Y2, Z2, X3, Y3, Z3, CenterArcDirection, AddDimension) ``` | |

| C# |  |
| --- | --- |
| ``` SketchSlot CreateSketchSlot(     System.int SlotCreationType,    System.int SlotLengthType,    System.double Width,    System.double X1,    System.double Y1,    System.double Z1,    System.double X2,    System.double Y2,    System.double Z2,    System.double X3,    System.double Y3,    System.double Z3,    System.int CenterArcDirection,    System.bool AddDimension ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` SketchSlot^ CreateSketchSlot(  &   System.int SlotCreationType, &   System.int SlotLengthType, &   System.double Width, &   System.double X1, &   System.double Y1, &   System.double Z1, &   System.double X2, &   System.double Y2, &   System.double Z2, &   System.double X3, &   System.double Y3, &   System.double Z3, &   System.int CenterArcDirection, &   System.bool AddDimension ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SlotCreationType*
:   Type of sketch slot as defined in swSketchSlotCreationType\_e

*SlotLengthType*
:   Type of length of sketch slot as defined in swSketchSlotLengthType\_e

*Width*
:   Width of sketch slot

*X1*
:   x coordinate of point 1

*Y1*
:   y coordinate of point 1

*Z1*
:   z coordinate of point 2

*X2*
:   x coordinate of point 2

*Y2*
:   y coordinate of point 2

*Z2*
:   z coordinate of point 2

*X3*
:   x coordinate of point 3

*Y3*
:   y coordinate of point 3

*Z3*
:   z coordinate of point 3

*CenterArcDirection*
:   * -1 = Clockwise (CW)* 1 = Counterclockwise (CCW)

*AddDimension*
:   True to automatically add dimensions, false to not

#### Return Value

[Sketch slot](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSlot.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::CreateSketchSlot.

# ![](dotnetimages/collapse.gif)Example

[Insert and Resize Sketch Slot (C#)](Insert_and_Resize_Sketch_Slot_Example_CSharp.htm)

[Insert and Resize Sketch Slot (VB.NET)](Insert_and_Resize_Sketch_Slot_Example_VBNET.htm)

[Insert and Resize Sketch Slot (VBA)](Insert_and_Resize_Sketch_Slot_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0