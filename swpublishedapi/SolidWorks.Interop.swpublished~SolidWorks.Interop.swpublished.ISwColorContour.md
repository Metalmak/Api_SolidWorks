<!-- source: swpublishedapi/SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Custom Interfaces API Help | Send comments on this topic. |
| ISwColorContour Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html) : ISwColorContour Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Obsolete. Superseded by [ISwColorContour1](SOLIDWORKS.Interop.swpublished~SOLIDWORKS.Interop.swpublished.ISwColorContour1.html).

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface ISwColorContour ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwColorContour ``` | |

| C# |  |
| --- | --- |
| ``` public interface ISwColorContour ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class ISwColorContour ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwColorContour.

# ![](dotnetimages/collapse.gif)Remarks

This SwColorContour object and its methods let your implemented interface:

* Render the model using colors that are application-defined at specific locations for criteria like temperature, thickness, stress, and so on.

  * Display values associated with the colors at the cursor location.

To use SwColorContour:

1. Implement the SOLIDWORKS SwColorContour interface.

   - Install your implemented interface in the SOLIDWORKS software using IModelDocExtension::InstallModelColorizer.

     - Remove your implemented interface from the SOLIDWORKS software using IModelDocExtension::RemoveModelColorizer when you want to stop your implemented interface.

NOTE: Only one color and display interface can be active at any one time. The last color and display interface installed is the active one. If you remove that color and display interface, then the color and display interface installed before it becomes the active color and display interface.

See SOLIDWORKS Help for details about SOLIDWORKS Curvature Display.

To use this interface in a SOLIDWORKS VB.NET or C# macro or add-in, see ComVisibleAttribute in VB.NET and C# Macros and Add-ins.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwColorContour Members](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished.ISwColorContour_members.html)

[SolidWorks.Interop.swpublished Namespace](SolidWorks.Interop.swpublished~SolidWorks.Interop.swpublished_namespace.html)