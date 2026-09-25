<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData~BoundingSketch.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| BoundingSketch Property (ICoreFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICoreFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData.html) : BoundingSketch Property (ICoreFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the bounding sketch for this core feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property BoundingSketch As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICoreFeatureData Dim value As Feature   instance.BoundingSketch = value   value = instance.BoundingSketch ``` | |

| C# |  |
| --- | --- |
| ``` Feature BoundingSketch {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property Feature^ BoundingSketch {    Feature^ get();    void set ( &   Feature^ value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Pointer to the [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CoreFeatureData::BoundingSketch.

# ![](dotnetimages/collapse.gif)Example

[Get Core Feature Data (VBA)](Get_Core_Feature_Example_VB.htm)

[Get Core Feature Data (C#)](Get_Core_Feature_Example_CSharp.htm)

[Get Core Feature Data (VB.NET)](Get_Core_Feature_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

See Accessing Selections that Define Features for additional details on using this property.

# ![](dotnetimages/collapse.gif)See Also

####

[ICoreFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData.html)

[ICoreFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICoreFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0