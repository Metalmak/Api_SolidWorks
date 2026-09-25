<!-- source: dsgnchkapi/SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck~RunDesignCheck.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Design Checker API Help | Send comments on this topic. |
| RunDesignCheck Method (ISWDesignCheck) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.dsgnchk Namespace](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk_namespace.html) > [ISWDesignCheck Interface](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck.html) : RunDesignCheck Method (ISWDesignCheck) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*StandardFileName*

*ReportFolderName*

*AddReportToDesignBinder*

*OverWriteReport*

Obsolete. Superseded by [ISWDesignCheck::RunDesignCheck2](SOLIDWORKS.Interop.dsgnchk~SOLIDWORKS.Interop.dsgnchk.ISWDesignCheck~RunDesignCheck2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RunDesignCheck( _    ByVal StandardFileName As System.String, _    ByVal ReportFolderName As System.String, _    ByVal AddReportToDesignBinder As System.Boolean, _    ByVal OverWriteReport As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISWDesignCheck Dim StandardFileName As System.String Dim ReportFolderName As System.String Dim AddReportToDesignBinder As System.Boolean Dim OverWriteReport As System.Boolean Dim value As System.Integer   value = instance.RunDesignCheck(StandardFileName, ReportFolderName, AddReportToDesignBinder, OverWriteReport) ``` | |

| C# |  |
| --- | --- |
| ``` System.int RunDesignCheck(     System.string StandardFileName,    System.string ReportFolderName,    System.bool AddReportToDesignBinder,    System.bool OverWriteReport ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int RunDesignCheck(  &   System.String^ StandardFileName, &   System.String^ ReportFolderName, &   System.bool AddReportToDesignBinder, &   System.bool OverWriteReport ) ``` | |

#### Parameters

*StandardFileName*

*ReportFolderName*

*AddReportToDesignBinder*

*OverWriteReport*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SWDesignCheck::RunDesignCheck.

# ![](dotnetimages/collapse.gif)See Also

####

[ISWDesignCheck Interface](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck.html)

[ISWDesignCheck Members](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck_members.html)