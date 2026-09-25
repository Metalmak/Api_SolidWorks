<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPatternFeature~PatternType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| PatternType Property (IDimXpertPatternFeature) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertPatternFeature Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPatternFeature.html) : PatternType Property (IDimXpertPatternFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the type of this DimXpert pattern feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property PatternType As swDimXpertFeatureType_e ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertPatternFeature Dim value As swDimXpertFeatureType_e   value = instance.PatternType ``` | |

| C# |  |
| --- | --- |
| ``` swDimXpertFeatureType_e PatternType {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property swDimXpertFeatureType_e PatternType {    swDimXpertFeatureType_e get(); } ``` | |

#### Property Value

Type of this DimXpert pattern feature as defined in [swDimXpertFeatureType\_e](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.swDimXpertFeatureType_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimXpertPatternFeature::PatternType.

# ![](dotnetimages/collapse.gif)Example

[Get and Set Pattern Example (C#)](Get_and_Set_Pattern_Example_CSharp.htm)

[Get and Set Pattern Example (VB.NET)](Get_and_Set_Pattern_Example_VBNET.htm)

[Get and Set Pattern Example (VBA)](Get_and_Set_Pattern_Example_VB.htm)

[Get DimXpert Feature Example (VBA)](Get_DimXpert_Feature_Example_VB.htm)

[Get DimXpert Feature Example (VB.NET)](Get_DimXpert_Feature_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertPatternFeature Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPatternFeature.html)

[IDimXpertPatternFeature Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPatternFeature_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0