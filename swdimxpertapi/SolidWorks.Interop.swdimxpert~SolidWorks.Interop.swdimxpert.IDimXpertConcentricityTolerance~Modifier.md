<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertConcentricityTolerance~Modifier.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| Modifier Property (IDimXpertConcentricityTolerance) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertConcentricityTolerance Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertConcentricityTolerance.html) : Modifier Property (IDimXpertConcentricityTolerance) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the material condition modifier for this DimXpert concentricity tolerance.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property Modifier As swDimXpertMaterialConditionModifier_e ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertConcentricityTolerance Dim value As swDimXpertMaterialConditionModifier_e   value = instance.Modifier ``` | |

| C# |  |
| --- | --- |
| ``` swDimXpertMaterialConditionModifier_e Modifier {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property swDimXpertMaterialConditionModifier_e Modifier {    swDimXpertMaterialConditionModifier_e get(); } ``` | |

#### Property Value

Material condition modifier as defined in [swDimXpertMaterialConditionModifier\_e](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.swDimXpertMaterialConditionModifier_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimXpertConcentricityTolerance::Modifier.

# ![](dotnetimages/collapse.gif)Example

[Get DimXpert Tolerance5 Example (VBA)](Get_DimXpert_Tolerance5_Example_VB.htm)

[Get DimXpert Tolerance5 Example (VB.NET)](Get_DimXpert_Tolerance5_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertConcentricityTolerance Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertConcentricityTolerance.html)

[IDimXpertConcentricityTolerance Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertConcentricityTolerance_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0