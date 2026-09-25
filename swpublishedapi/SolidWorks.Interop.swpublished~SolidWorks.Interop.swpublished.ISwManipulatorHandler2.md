<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| ISwManipulatorHandler2 Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler2_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) : ISwManipulatorHandler2 Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Must be implemented by an add-in application to interact with a manipulator.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface ISwManipulatorHandler2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwManipulatorHandler2 ``` | |

| C# |  |
| --- | --- |
| ``` public interface ISwManipulatorHandler2 ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class ISwManipulatorHandler2 ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwManipulatorHandler2.

# ![](dotnetimages/collapse.gif)Example

[Insert and Use Plane with Manipulator (VBA)](Insert_and_Use_Plane_with_Manipulator_Example_VB.htm)

[Insert and Use Plane with Manipulator (VB.NET)](Insert_and_Use_Plane_with_Manipulator_Example_VBNET.htm)

[Insert and Use Plane with Manipulator (C#)](Insert_and_Use_Plane_with_Manipulator_Example_CSharp.htm)

[Create Triad Manipulator (VBA)](Create_Triad_Manipulator_Example_VB.htm)

[Create Triad Manipulator (VB.NET)](Create_Triad_Manipulator_Example_VBNET.htm)

[Create Triad Manipulator (C#)](Create_Triad_Manipulator_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

To use this interface in a SOLIDWORKS VB.NET or C# macro or add-in, see ComVisibleAttribute in VB.NET and C# Macros and Add-ins.

The add-in application performs such actions as:

* Defining how a manipulator moves. For example, the add-in application has the manipulator follow a surface in order to place an image on that surface.

  * Providing any temporary graphics associated with manipulator. For example, to display a temporary body in a part, the add-in application must call IBody2::Display3.

    * Applying transforms using IBody2::ApplyTransform.

To create a manipulator, first create the SwManipulatorHandler2 object and then create the IManipulator object.

See Manipulators for details.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwManipulatorHandler2 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwManipulatorHandler2_members.html)

[SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html)

IDragArrowManipulator Interface

ITriadManipulator Interface

IPlaneManipulator interface