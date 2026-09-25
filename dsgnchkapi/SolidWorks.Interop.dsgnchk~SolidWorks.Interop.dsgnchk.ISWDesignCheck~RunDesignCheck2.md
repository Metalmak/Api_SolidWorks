<!-- source: dsgnchkapi/SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck~RunDesignCheck2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Design Checker API Help | Send comments on this topic. |
| RunDesignCheck2 Method (ISWDesignCheck) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.dsgnchk Namespace](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk_namespace.html) > [ISWDesignCheck Interface](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck.html) : RunDesignCheck2 Method (ISWDesignCheck) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*StandardFileName*
:   Path and filename of SOLIDWORKS Design Checker standards document

*ReportFolderName*
:   Name of report

    **NOTE:** A filename extension of **.dxp** is automatically appended to the specified filename. The report is an XML file.

*AddReportToDesignBinder*
:   True to add the report to the Design Binder, false to not

*OverWriteReport*
:   True to overwrite any existing report of the same name in the Design Binder, false to not

*bCanViewReportOnSave*
:   True to display the report when saved, false to not

Obsolete. Superseded by [ISWDesignCheck::RunDesignCheck3](SOLIDWORKS.Interop.dsgnchk~SOLIDWORKS.Interop.dsgnchk.ISWDesignCheck~RunDesignCheck3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RunDesignCheck2( _    ByVal StandardFileName As System.String, _    ByVal ReportFolderName As System.String, _    ByVal AddReportToDesignBinder As System.Boolean, _    ByVal OverWriteReport As System.Boolean, _    ByVal bCanViewReportOnSave As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISWDesignCheck Dim StandardFileName As System.String Dim ReportFolderName As System.String Dim AddReportToDesignBinder As System.Boolean Dim OverWriteReport As System.Boolean Dim bCanViewReportOnSave As System.Boolean Dim value As System.Integer   value = instance.RunDesignCheck2(StandardFileName, ReportFolderName, AddReportToDesignBinder, OverWriteReport, bCanViewReportOnSave) ``` | |

| C# |  |
| --- | --- |
| ``` System.int RunDesignCheck2(     System.string StandardFileName,    System.string ReportFolderName,    System.bool AddReportToDesignBinder,    System.bool OverWriteReport,    System.bool bCanViewReportOnSave ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int RunDesignCheck2(  &   System.String^ StandardFileName, &   System.String^ ReportFolderName, &   System.bool AddReportToDesignBinder, &   System.bool OverWriteReport, &   System.bool bCanViewReportOnSave ) ``` | |

#### Parameters

*StandardFileName*
:   Path and filename of SOLIDWORKS Design Checker standards document

*ReportFolderName*
:   Name of report

    **NOTE:** A filename extension of **.dxp** is automatically appended to the specified filename. The report is an XML file.

*AddReportToDesignBinder*
:   True to add the report to the Design Binder, false to not

*OverWriteReport*
:   True to overwrite any existing report of the same name in the Design Binder, false to not

*bCanViewReportOnSave*
:   True to display the report when saved, false to not

#### Return Value

Error code as defined in [dsgnchkError\_e](SOLIDWORKS.Interop.dsgnchk~SOLIDWORKS.Interop.dsgnchk.dsgnchkError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SWDesignCheck::RunDesignCheck2.

# ![](dotnetimages/collapse.gif)Remarks

This method can also add a new, or overwrite an existing, report to the Design Binder.

# ![](dotnetimages/collapse.gif)See Also

####

[ISWDesignCheck Interface](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck.html)

[ISWDesignCheck Members](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0