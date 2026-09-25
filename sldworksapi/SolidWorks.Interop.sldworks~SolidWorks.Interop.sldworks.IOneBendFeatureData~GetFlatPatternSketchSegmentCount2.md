<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IOneBendFeatureData~GetFlatPatternSketchSegmentCount2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetFlatPatternSketchSegmentCount2 Method (IOneBendFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IOneBendFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IOneBendFeatureData.html) : GetFlatPatternSketchSegmentCount2 Method (IOneBendFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the number of sketch segments, including bend lines, in this bend.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetFlatPatternSketchSegmentCount2() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IOneBendFeatureData Dim value As System.Integer   value = instance.GetFlatPatternSketchSegmentCount2() ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetFlatPatternSketchSegmentCount2() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetFlatPatternSketchSegmentCount2(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Number of sketch segments in this bend

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See OneBendFeatureData::GetFlatPatternSketchSegmentCount2.

# ![](dotnetimages/collapse.gif)Example

[Get Names of Sketch Segments (VBA)](Get_Names_of_Sketch_Segments_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call this method to populate SegmentsCount in [IOneBendFeatureData::IFlatPatternSketchSegments2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IOneBendFeatureData~IFlatPatternSketchSegments2.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IOneBendFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IOneBendFeatureData.html)

[IOneBendFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IOneBendFeatureData_members.html)

[IOneBendFeatureData::FlatPatternSketchSegments2 Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IOneBendFeatureData~FlatPatternSketchSegments2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2012 SP02, Revision Number 20.2