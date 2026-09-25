<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFillPatternFeatureData~FeaturesToPatternType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeaturesToPatternType Property (IFillPatternFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFillPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFillPatternFeatureData.html) : FeaturesToPatternType Property (IFillPatternFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the type of object to pattern in this fill pattern feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property FeaturesToPatternType As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFillPatternFeatureData Dim value As System.Integer   instance.FeaturesToPatternType = value   value = instance.FeaturesToPatternType ``` | |

| C# |  |
| --- | --- |
| ``` System.int FeaturesToPatternType {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int FeaturesToPatternType {    System.int get();    void set ( &   System.int value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Type of object to pattern as defined in swFeaturesToPatternType\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FillPatternFeatureData::FeaturesToPatternType.

# ![](dotnetimages/collapse.gif)Example

See the [IFillPatternFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFillPatternFeatureData.html) example.

# ![](dotnetimages/collapse.gif)Remarks

| If this property is set to... | Then call... |
| --- | --- |
| swFeaturesToPatternType\_e.swFeaturesToPatternCreateSeedCut | [IFillPatternFeatureData::CreateSeedCutType](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFillPatternFeatureData~CreateSeedCutType.html) to get or set the type of seed cut to pattern |
| swFeaturesToPatternType\_e.swFeaturesToPatternSelectedFeatures | * [IFillPatternFeatureData::PatternFeatureArray](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFillPatternFeatureData~PatternFeatureArray.html) to get or set the array of features to pattern* [IFillPatternFeatureData::PatternFaceArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFillPatternFeatureData~PatternFaceArray.html) to get or set the array of faces to pattern* [IFillPatternFeatureData::PatternBodyArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFillPatternFeatureData~PatternBodyArray.html) to get or set the array of bodies to pattern |

# ![](dotnetimages/collapse.gif)See Also

####

[IFillPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFillPatternFeatureData.html)

[IFillPatternFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFillPatternFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2014 FCS, Revision Number 22.0