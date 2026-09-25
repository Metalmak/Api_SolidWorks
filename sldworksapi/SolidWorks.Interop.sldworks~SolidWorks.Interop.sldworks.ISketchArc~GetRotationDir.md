<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchArc~GetRotationDir.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetRotationDir Method (ISketchArc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchArc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchArc.html) : GetRotationDir Method (ISketchArc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the rotation direction of this sketch arc.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetRotationDir() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchArc Dim value As System.Integer   value = instance.GetRotationDir() ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetRotationDir() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetRotationDir(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Rotation direction with respect to the normal of the arc's sketch plane (counterclockwise = 1, clockwise = -1) (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchArc::GetRotationDir.

# ![](dotnetimages/collapse.gif)Example

See the [ISketchArc](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchArc.html) examples.

# ![](dotnetimages/collapse.gif)Example

[Get All Elements in Sketch (VBA)](Get_All_Elements_of_Sketch_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method determines the direction that the sketch proceeds around this arc, beginning at the arc's start point and ending at the arc's end point. The direction is with respect to the normal of the arc's sketch plane and not with respect to the viewer.

| If the normal to the arc's sketch plane is... | And the normal to the arc is... | And this method returns... | It means that... |
| --- | --- | --- | --- |
| (0, 0, -1) | (0, 0, 1) | 1 (counterclockwise) | With respect to its sketch plane's normal (from behind the screen), the arc travels counterclockwise from its start point to its end point.  Note that from the perspective of the viewer (in front of the screen), the arc travels clockwise from its start point to its end point. |

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchArc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchArc.html)

[ISketchArc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchArc_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 99, datecode 1999207