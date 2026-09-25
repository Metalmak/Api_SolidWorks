<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour1.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| ISwColorContour1 Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour1_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) : ISwColorContour1 Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to the color and display values of curvature in a SOLIDWORKS model.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface ISwColorContour1 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwColorContour1 ``` | |

| C# |  |
| --- | --- |
| ``` public interface ISwColorContour1 ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class ISwColorContour1 ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwColorContour1.

# ![](dotnetimages/collapse.gif)Example

[Custom Colorize a Model Example (C#)](Custom_Colorize_a_Model_Example_CSharp.htm)

[Custom Colorize a Model Example (VB.NET)](Custom_Colorize_a_Model_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

When implemented, the methods of this interface allow you to assign colors and display values of curvature in a SOLIDWORKS model.

To use ISwColorContour1:

1. Implement the ISwColorContour1 interface in an add-in class.

   - Install the implemented interface in the SOLIDWORKS software using IModelDocExtension::InstallModelColorizer.

     - Run the add-in and open a model document in SOLIDWORKS.

       - In SOLIDWORKS select **View > Display > Curvature.** The model is colorized by the implemented interface.

         - When you finalize the application, remove the implemented interface from the SOLIDWORKS software using IModelDocExtension::RemoveModelColorizer.

NOTE: Only one color and display interface can be active at any one time. The last color and display interface installed is the active one. If you remove that color and display interface, then the color and display interface installed before it becomes the active color and display interface.

This interface overrides the color and display functionality of the SOLIDWORKS Curvature tool. See SOLIDWORKS Help for details about the SOLIDWORKS Curvature tool.

To use this interface in a SOLIDWORKS VB.NET or C# macro or add-in, see ComVisibleAttribute in VB.NET and C# Macros and Add-ins.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwColorContour1 Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour1_members.html)

[SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html)