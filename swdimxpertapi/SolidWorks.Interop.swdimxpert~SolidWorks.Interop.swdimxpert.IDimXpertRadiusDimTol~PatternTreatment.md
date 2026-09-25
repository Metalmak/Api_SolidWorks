<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertRadiusDimTol~PatternTreatment.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| PatternTreatment Property (IDimXpertRadiusDimTol) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertRadiusDimTol Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertRadiusDimTol.html) : PatternTreatment Property (IDimXpertRadiusDimTol) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the pattern treatment for this DimXpert radius dimension tolerance.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property PatternTreatment As swDimXpertPatternTreatmentType_e ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertRadiusDimTol Dim value As swDimXpertPatternTreatmentType_e   value = instance.PatternTreatment ``` | |

| C# |  |
| --- | --- |
| ``` swDimXpertPatternTreatmentType_e PatternTreatment {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property swDimXpertPatternTreatmentType_e PatternTreatment {    swDimXpertPatternTreatmentType_e get(); } ``` | |

#### Property Value

Pattern treatment type as defined in [swDimXpertPatternTreatmentType\_e](SOLIDWORKS.Interop.swdimxpert~SOLIDWORKS.Interop.swdimxpert.swDimXpertPatternTreatmentType_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimXpertRadiusDimTol::PatternTreatment.

# ![](dotnetimages/collapse.gif)Example

[Get DimXpert Tolerance2 Example (VBA)](Get_DimXpert_Tolerance2_Example_VB.htm)

[Get DimXpert Tolerance2 Example (VB.NET)](Get_DimXpert_Tolerance2_Example_VBNET.htm)

[Get DimXpert Features and Annotations in a Model Example (C#)](Get_DimXpert_Features_and_Annotations_in_a_Model_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertRadiusDimTol Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertRadiusDimTol.html)

[IDimXpertRadiusDimTol Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertRadiusDimTol_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0