<!-- source: swinspectionapi/SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IInspectionAddinMgr~AddCharacteristics.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Inspection API Help | Send comments on this topic. |
| AddCharacteristics Method (IInspectionAddinMgr) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swinspectionAddIn Namespace](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn_namespace.html) > [IInspectionAddinMgr Interface](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IInspectionAddinMgr.html) : AddCharacteristics Method (IInspectionAddinMgr) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*AnnotationsIn*
:   Array of annotations

Adds characteristics for the specified annotations.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddCharacteristics( _    ByRef AnnotationsIn As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IInspectionAddinMgr Dim AnnotationsIn As System.Object Dim value As System.Object   value = instance.AddCharacteristics(AnnotationsIn) ``` | |

| C# |  |
| --- | --- |
| ``` System.object AddCharacteristics(     ref System.object AnnotationsIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ AddCharacteristics(  &   System.Object^% AnnotationsIn ) ``` | |

#### Parameters

*AnnotationsIn*
:   Array of annotations

#### Return Value

[ICharacteristicsData](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.ICharacteristicsData.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See InspectionAddinMgr methods.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [IInspectionProjectData::Extraction](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IInspectionProjectData~Extraction.html) is set to [swiCharacteristicInfoExtraction\_e](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.swiCharacteristicInfoExtraction_e.html).swiExtraction\_Manual.

# ![](dotnetimages/collapse.gif)See Also

####

[IInspectionAddinMgr Interface](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IInspectionAddinMgr.html)

[IInspectionAddinMgr Members](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IInspectionAddinMgr_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Inspection API 2022 FCS