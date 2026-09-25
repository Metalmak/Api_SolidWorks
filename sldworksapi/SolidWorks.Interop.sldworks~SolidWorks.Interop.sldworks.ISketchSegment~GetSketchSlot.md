<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment~GetSketchSlot.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSketchSlot Method (ISketchSegment) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchSegment Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment.html) : GetSketchSlot Method (ISketchSegment) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets sketch slot with which this sketch segment is associated.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSketchSlot() As SketchSlot ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchSegment Dim value As SketchSlot   value = instance.GetSketchSlot() ``` | |

| C# |  |
| --- | --- |
| ``` SketchSlot GetSketchSlot() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` SketchSlot^ GetSketchSlot(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

[Sketch slot](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSlot.html) if the sketch segment is associated with a sketch slot, or null if the sketch segment is not associated with a sketch slot

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchSegment::GetSketchSlot.

# ![](dotnetimages/collapse.gif)Example

[Get Sketch Slot Using Sketch Point and Segment (C#)](Get_Sketch_Slot_Using_Sketch_Point_and_Segment_Example_CSharp.htm)

[Get Sketch Slot Using Sketch Point and Segment (VB.NET)](Get_Sketch_Slot_Using_Sketch_Point_and_Segment_Example_VBNET.htm)

[Get Sketch Slot Using Sketch Point and Segment (VBA)](Get_Sketch_Slot_Using_Sketch_Point_and_Segment_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchSegment Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment.html)

[ISketchSegment Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchSegment_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 SP2, Revision Number 17.2