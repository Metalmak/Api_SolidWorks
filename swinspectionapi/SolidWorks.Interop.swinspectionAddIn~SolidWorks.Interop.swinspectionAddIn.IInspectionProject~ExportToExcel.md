<!-- source: swinspectionapi/SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IInspectionProject~ExportToExcel.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Inspection API Help | Send comments on this topic. |
| ExportToExcel Method (IInspectionProject) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swinspectionAddIn Namespace](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn_namespace.html) > [IInspectionProject Interface](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IInspectionProject.html) : ExportToExcel Method (IInspectionProject) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*TemplatePath*
:   Full path name of the inspection report template to use (see **Remarks**)

*FilePath*
:   Full path name of the Microsoft Excel file to export

*Multisheet*
:   True if multisheet, false if not

Exports the inspection report to Microsoft Excel.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ExportToExcel( _    ByVal TemplatePath As System.String, _    ByVal FilePath As System.String, _    ByVal Multisheet As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IInspectionProject Dim TemplatePath As System.String Dim FilePath As System.String Dim Multisheet As System.Boolean Dim value As System.Boolean   value = instance.ExportToExcel(TemplatePath, FilePath, Multisheet) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool ExportToExcel(     System.string TemplatePath,    System.string FilePath,    System.bool Multisheet ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool ExportToExcel(  &   System.String^ TemplatePath, &   System.String^ FilePath, &   System.bool Multisheet ) ``` | |

#### Parameters

*TemplatePath*
:   Full path name of the inspection report template to use (see **Remarks**)

*FilePath*
:   Full path name of the Microsoft Excel file to export

*Multisheet*
:   True if multisheet, false if not

#### Return Value

True if export is successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See InspectionProject methods.

# ![](dotnetimages/collapse.gif)Remarks

The templates are installed in **c:\ProgramData\SOLIDWORKS\SOLIDWORKS Inspection 2022 Addin\Templates**.

# ![](dotnetimages/collapse.gif)See Also

####

[IInspectionProject Interface](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IInspectionProject.html)

[IInspectionProject Members](SolidWorks.Interop.swinspectionAddIn~SolidWorks.Interop.swinspectionAddIn.IInspectionProject_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Inspection API 2022 FCS