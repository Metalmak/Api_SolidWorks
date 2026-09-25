<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEndCapFeatureData~UseThicknessRatioForOffset.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| UseThicknessRatioForOffset Property (IEndCapFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IEndCapFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEndCapFeatureData.html) : UseThicknessRatioForOffset Property (IEndCapFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether a ratio of the thickness is used to specify the offset for this end-cap feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property UseThicknessRatioForOffset As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEndCapFeatureData Dim value As System.Boolean   instance.UseThicknessRatioForOffset = value   value = instance.UseThicknessRatioForOffset ``` | |

| C# |  |
| --- | --- |
| ``` System.bool UseThicknessRatioForOffset {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool UseThicknessRatioForOffset {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to use a ratio of the thickness, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EndCapFeatureData::UseThicknessRatioForOffset.

# ![](dotnetimages/collapse.gif)Example

See the [IEndCapFeatureData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEndCapFeatureData.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| **If this property is set to...** | **Then you can use...** |
| True | [IEndCapFeatureData::ThicknessRatioForOffset](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEndCapFeatureData~ThicknessRatioForOffset.html) to set the offset distance of the end cap as a ratio of the thickness of the structural member being capped. |
| False | [IEndCapFeatureData::OffsetDistance](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEndCapFeatureData~OffsetDistance.html) to set the offset distance for this end-cap feature. |

# ![](dotnetimages/collapse.gif)See Also

####

[IEndCapFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEndCapFeatureData.html)

[IEndCapFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEndCapFeatureData_members.html)

[IEndCapFeatureData::Thickness Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEndCapFeatureData~Thickness.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0