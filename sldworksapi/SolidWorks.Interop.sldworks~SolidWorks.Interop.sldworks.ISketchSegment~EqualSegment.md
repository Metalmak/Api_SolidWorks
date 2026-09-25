<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~EqualSegment.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EqualSegment Method (ISketchSegment) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchSegment Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment.html) : EqualSegment Method (ISketchSegment) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SketchType*
:   Type of entity with which to divide this sketch segment as defined in swSketchSegmentType\_e

*SegmentPoints*
:   2 <= Number of sketchType entities into which to divide this sketch segment <= 100

Divides this sketch segment into equally spaced sketch segments or points.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function EqualSegment( _    ByVal SketchType As System.Integer, _    ByVal SegmentPoints As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchSegment Dim SketchType As System.Integer Dim SegmentPoints As System.Integer Dim value As System.Boolean   value = instance.EqualSegment(SketchType, SegmentPoints) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool EqualSegment(     System.int SketchType,    System.int SegmentPoints ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool EqualSegment(  &   System.int SketchType, &   System.int SegmentPoints ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*SketchType*
:   Type of entity with which to divide this sketch segment as defined in swSketchSegmentType\_e

*SegmentPoints*
:   2 <= Number of sketchType entities into which to divide this sketch segment <= 100

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchSegment::EqualSegment.

# ![](dotnetimages/collapse.gif)Example

[Divide Sketch Segment (VBA)](Divide_Sketch_Segment_Example_VB.htm)

[Divide Sketch Segment (VB.NET)](Divide_Sketch_Segment_Example_VBNET.htm)

[Divide Sketch Segment (C#)](Divide_Sketch_Segment_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchSegment Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment.html)

[ISketchSegment Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0