<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPatternFeature~IGetSubFeatures.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| IGetSubFeatures Method (IDimXpertPatternFeature) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertPatternFeature Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPatternFeature.html) : IGetSubFeatures Method (IDimXpertPatternFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Count*
:   Number of sub-features in this DimXpert pattern feature

Gets all of the sub-features of this DimXpert pattern feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetSubFeatures( _    ByVal Count As System.Integer _ ) As DimXpertFeature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertPatternFeature Dim Count As System.Integer Dim value As DimXpertFeature   value = instance.IGetSubFeatures(Count) ``` | |

| C# |  |
| --- | --- |
| ``` DimXpertFeature IGetSubFeatures(     System.int Count ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` DimXpertFeature^ IGetSubFeatures(  &   System.int Count ) ``` | |

#### Parameters

*Count*
:   Number of sub-features in this DimXpert pattern feature

#### Return Value

- in-process, unmanaged C++: Pointer to an array of [IDimXpertFeature](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.IDimXpertFeature.html)- VBA, VB.NET, C#, and C++/CLI: Not supported

# ![](dotnetimages/collapse.gif)Remarks

This method returns all sub-features of the pattern feature. All of the sub-features returned by this method do not appear on the DimXpertManager tab of the Management Panel. Functional geometry sub-features such as planes and cylinders that represent each individual face of a part are for internal use only. These sub-features do not appear in the DimXpertManager tree. However, manufacturing sub-features that are significant for downstream machining and inspection of the pattern do appear in the DimXpertManager tree.

For example, the sub-features of a simple hole are related to functional geometry and are not listed in the DimXpertManager tree. However, the sub-features of a hole pattern are manufacturing features (e.g., simple holes) that are significant for downstream processes. These manufacturing features are listed in the DimXpertManager tree.

See In-process Methods for details about this type of method.

Before calling this method, call [IDimXpertPatternFeature::GetSubFeatureCount](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.IDimXpertPatternFeature~GetSubFeatureCount.html) to get the value for the Count parameter.

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertPatternFeature Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPatternFeature.html)

[IDimXpertPatternFeature Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertPatternFeature_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0