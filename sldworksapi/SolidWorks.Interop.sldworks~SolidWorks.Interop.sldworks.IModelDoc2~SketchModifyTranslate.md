<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SketchModifyTranslate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SketchModifyTranslate Method (IModelDoc2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html) : SketchModifyTranslate Method (IModelDoc2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*StartX*
:   X sketch value defining the from-position

*StartY*
:   Y sketch value defining the from-position

*EndX*
:   X sketch value defining the to-position

*EndY*
:   Y sketch value defining the to-position

Translates the coordinate system of the active or selected sketch.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SketchModifyTranslate( _    ByVal StartX As System.Double, _    ByVal StartY As System.Double, _    ByVal EndX As System.Double, _    ByVal EndY As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDoc2 Dim StartX As System.Double Dim StartY As System.Double Dim EndX As System.Double Dim EndY As System.Double   instance.SketchModifyTranslate(StartX, StartY, EndX, EndY) ``` | |

| C# |  |
| --- | --- |
| ``` void SketchModifyTranslate(     System.double StartX,    System.double StartY,    System.double EndX,    System.double EndY ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SketchModifyTranslate(  &   System.double StartX, &   System.double StartY, &   System.double EndX, &   System.double EndY ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*StartX*
:   X sketch value defining the from-position

*StartY*
:   Y sketch value defining the from-position

*EndX*
:   X sketch value defining the to-position

*EndY*
:   Y sketch value defining the to-position

#### Return Value

The sketch is translated from the XY start point position to the XY end point position.

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDoc2::SketchModifyTranslate.

# ![](dotnetimages/collapse.gif)Example

[Translate Sketch (VBA)](Translate_Sketch_Example_VB.htm)

[Translate Sketch (VB.NET)](Translate_Sketch_Example_VBNET.htm)

[Translate Sketch (C#)](Translate_Sketch_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDoc2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2.html)

[IModelDoc2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2_members.html)

[IModelDoc2::ToolsSketchTranslate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ToolsSketchTranslate.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0