<!-- source: swinspectionapi/SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IInspectionAddinMgr~CreateInspectionProjectData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Inspection API Help | Send comments on this topic. |
| CreateInspectionProjectData Method (IInspectionAddinMgr) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swinspectionAddIn Namespace](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn_namespace.html) > [IInspectionAddinMgr Interface](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IInspectionAddinMgr.html) : CreateInspectionProjectData Method (IInspectionAddinMgr) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*TemplatePathIn*
:   Full path name of inspection project template (see **Remarks**)

Creates inspection project data.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateInspectionProjectData( _    ByVal TemplatePathIn As System.String _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IInspectionAddinMgr Dim TemplatePathIn As System.String Dim value As System.Object   value = instance.CreateInspectionProjectData(TemplatePathIn) ``` | |

| C# |  |
| --- | --- |
| ``` System.object CreateInspectionProjectData(     System.string TemplatePathIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ CreateInspectionProjectData(  &   System.String^ TemplatePathIn ) ``` | |

#### Parameters

*TemplatePathIn*
:   Full path name of inspection project template (see **Remarks**)

#### Return Value

[IInspectionProjectData](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IInspectionProjectData.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See InspectionAddinMgr methods.

# ![](dotnetimages/collapse.gif)Remarks

The templates are installed in **c:\ProgramData\SOLIDWORKS\SOLIDWORKS Inspection 2022 Addin\Templates**.

# ![](dotnetimages/collapse.gif)See Also

####

[IInspectionAddinMgr Interface](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IInspectionAddinMgr.html)

[IInspectionAddinMgr Members](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IInspectionAddinMgr_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Inspection API 2022 FCS