<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMGussetFeatureData~FilletInnerCorners.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FilletInnerCorners Property (ISMGussetFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISMGussetFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMGussetFeatureData.html) : FilletInnerCorners Property (ISMGussetFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to fillet the inner corners of this gusset.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property FilletInnerCorners As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISMGussetFeatureData Dim value As System.Boolean   instance.FilletInnerCorners = value   value = instance.FilletInnerCorners ``` | |

| C# |  |
| --- | --- |
| ``` System.bool FilletInnerCorners {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool FilletInnerCorners {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to fillet the inner corners of this gusset, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SMGussetFeatureData::FilletInnerCorners.

# ![](dotnetimages/collapse.gif)Example

See the examples for [ISMGussetFeatureData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISMGussetFeatureData.html).

# ![](dotnetimages/collapse.gif)Remarks

After setting this property, set [ISMGussetFeatureData::InnerCornerFilletRadius](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISMGussetFeatureData~InnerCornerFilletRadius.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISMGussetFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMGussetFeatureData.html)

[ISMGussetFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMGussetFeatureData_members.html)

[ISMGussetFeatureData::FilletOuterCorners Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMGussetFeatureData~FilletOuterCorners.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0