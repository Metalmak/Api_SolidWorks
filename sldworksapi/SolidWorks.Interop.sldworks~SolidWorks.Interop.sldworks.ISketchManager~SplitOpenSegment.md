<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SplitOpenSegment.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SplitOpenSegment Method (ISketchManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : SplitOpenSegment Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X*
:   X coordinate of the point that splits the sketch segment in two

*Y*
:   Y coordinate of the point that splits the sketch segment in two

*Z*
:   Z coordinate of the point that splits the sketch segment in two

Splits the selected open sketch segment into two sketch segments.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SplitOpenSegment( _    ByVal X As System.Double, _    ByVal Y As System.Double, _    ByVal Z As System.Double _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim value As System.Object   value = instance.SplitOpenSegment(X, Y, Z) ``` | |

| C# |  |
| --- | --- |
| ``` System.object SplitOpenSegment(     System.double X,    System.double Y,    System.double Z ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ SplitOpenSegment(  &   System.double X, &   System.double Y, &   System.double Z ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*X*
:   X coordinate of the point that splits the sketch segment in two

*Y*
:   Y coordinate of the point that splits the sketch segment in two

*Z*
:   Z coordinate of the point that splits the sketch segment in two

#### Return Value

Array of [sketch segments](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchSegment.html) of the now split formerly open sketch skegment

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::SplitOpenSegment.

# ![](dotnetimages/collapse.gif)Example

[Split Open Sketch Segment (VBA)](Split_Open_Sketch_Segment_Example_VB.htm)

[Split Open Sketch Segment (VB.NET)](Split_Open_Sketch_Segment_Example_VBNET.htm)

[Split Open Sketch Segment (C#)](Split_Open_Sketch_Segment_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, be sure to disable snapping by either:

* De-selecting **System Options > Sketch > Relations/Snaps > Enable snapping**

    - or -

* Calling [ISldWorks::SetUserPreferenceToggle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~SetUserPreferenceToggle.html)(swUserPreferenceToggle\_e.swSketchInference, false).

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

[ISketchManager::SplitClosedSegment Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~SplitClosedSegment.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0