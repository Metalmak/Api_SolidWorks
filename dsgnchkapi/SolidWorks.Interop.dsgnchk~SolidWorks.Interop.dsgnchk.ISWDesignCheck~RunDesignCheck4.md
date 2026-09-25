<!-- source: dsgnchkapi/SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck~RunDesignCheck4.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Design Checker API Help | Send comments on this topic. |
| RunDesignCheck4 Method (ISWDesignCheck) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.dsgnchk Namespace](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk_namespace.html) > [ISWDesignCheck Interface](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck.html) : RunDesignCheck4 Method (ISWDesignCheck) |

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
:   Path and folder name for pre- and post-condition reports (see **Remarks**)

*AddReportToDesignBinder*
:   True to add the report to the Design Binder, false to not

*OverWriteReport*
:   True to overwrite any existing report of the same name in the Design Binder, false to not

*AutoCorrect*
:   True to autocorrect all failures discovered by Design Checker, false to not

Obsolete. Superseded by [ISWDesignCheck::RunDesignCheck5](SOLIDWORKS.Interop.dsgnchk~SOLIDWORKS.Interop.dsgnchk.ISWDesignCheck~RunDesignCheck5.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RunDesignCheck4( _    ByVal StandardFileName As System.String, _    ByVal ReportFolderName As System.String, _    ByVal AddReportToDesignBinder As System.Boolean, _    ByVal OverWriteReport As System.Boolean, _    ByVal AutoCorrect As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISWDesignCheck Dim StandardFileName As System.String Dim ReportFolderName As System.String Dim AddReportToDesignBinder As System.Boolean Dim OverWriteReport As System.Boolean Dim AutoCorrect As System.Boolean Dim value As System.Integer   value = instance.RunDesignCheck4(StandardFileName, ReportFolderName, AddReportToDesignBinder, OverWriteReport, AutoCorrect) ``` | |

| C# |  |
| --- | --- |
| ``` System.int RunDesignCheck4(     System.string StandardFileName,    System.string ReportFolderName,    System.bool AddReportToDesignBinder,    System.bool OverWriteReport,    System.bool AutoCorrect ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int RunDesignCheck4(  &   System.String^ StandardFileName, &   System.String^ ReportFolderName, &   System.bool AddReportToDesignBinder, &   System.bool OverWriteReport, &   System.bool AutoCorrect ) ``` | |

#### Parameters

*StandardFileName*
:   Path and filename of SOLIDWORKS Design Checker standards document

*ReportFolderName*
:   Path and folder name for pre- and post-condition reports (see **Remarks**)

*AddReportToDesignBinder*
:   True to add the report to the Design Binder, false to not

*OverWriteReport*
:   True to overwrite any existing report of the same name in the Design Binder, false to not

*AutoCorrect*
:   True to autocorrect all failures discovered by Design Checker, false to not

#### Return Value

Error code as defined in [dsgnchkError\_e](SOLIDWORKS.Interop.dsgnchk~SOLIDWORKS.Interop.dsgnchk.dsgnchkError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SWDesignCheck::RunDesignCheck4.

# ![](dotnetimages/collapse.gif)Example

[Run SOLIDWORKS Design Checker (C#)](Run_SOLIDWORKS_Design_Checker_Example_CSharp.htm)

[Run SOLIDWORKS Design Checker (VB.NET)](Run_SOLIDWORKS_Design_Checker_Example_VBNET.htm)

[Run SOLIDWORKS Design Checker (VBA)](Run_SOLIDWORKS_Design_Checker_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The date and time are automatically appended to the name of the folder specified for ReportFolderName. For example, if you specified **"c:\test\Food Processor"** for ReportFolderName and you ran your macro on July 28, 2009 at 8:30 a.m., then **c:\test\Food Processor\_7\_28\_2009\_8:30** is the name of the folder created. **Post-Correction Result** and **Pre-Correction Result** subfolders are also created, depending on the value specified for AutoCorrect. The post- and pre-condition reports are created in these subfolders.

|  |  |
| --- | --- |
| **If AutoCorrect is set to...** | **Then these reports are created...** |
| True | Design Binder: Post-Correction Result.dxpand Pre-Correction Result.dxp  **Post-Correction Result** and **Pre-Correction Result**subfolders: SWDCReport.xml |
| False | Design Binder: Pre-Correction Result.dxp **Pre-Correction Result** subfolder: SWDCReport.xml |

# ![](dotnetimages/collapse.gif)See Also

####

[ISWDesignCheck Interface](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck.html)

[ISWDesignCheck Members](SolidWorks.Interop.dsgnchk~SolidWorks.Interop.dsgnchk.ISWDesignCheck_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0