<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureStatistics~FeatureUpdateTimes.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureUpdateTimes Property (IFeatureStatistics) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureStatistics Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureStatistics.html) : FeatureUpdateTimes Property (IFeatureStatistics) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the times, in seconds, it takes to update (rebuild) each feature in a part document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property FeatureUpdateTimes As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureStatistics Dim value As System.Object   value = instance.FeatureUpdateTimes ``` | |

| C# |  |
| --- | --- |
| ``` System.object FeatureUpdateTimes {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.Object^ FeatureUpdateTimes {    System.Object^ get(); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Array of times, in seconds, it takes to udpate (rebuild) each feature in a part document

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureStatistics::FeatureUpdateTimes.

# ![](dotnetimages/collapse.gif)Example

[Get Part's Feature Statistics (VB.NET)](Get_Part%27s_Feature_Statistics_Example_VBNET.htm)

[Get Part's Feature Statistics (VBA)](Get_Part%27s_Feature_Statistics_Example_VB.htm)

[Get Part's Feature Statistics (C#)](Get_Part%27s_Feature_Statistics_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureStatistics Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureStatistics.html)

[IFeatureStatistics Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureStatistics_members.html)

[IFeatureStatistics::FeatureUpdatePercentageTimes Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureStatistics~FeatureUpdatePercentageTimes.html)

[IFeatureStatistics::TotalRebuildTime Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureStatistics~TotalRebuildTime.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0