<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExportPdfData~SetSheets.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetSheets Method (IExportPdfData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IExportPdfData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExportPdfData.html) : SetSheets Method (IExportPdfData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Which*
:   Drawing sheets to export to PDF as defined in swExportDataSheetsToExport\_e

*Sheets*
:   Array of the names of the drawing sheets to export

Sets the drawing [sheets](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISheet.html) to export.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetSheets( _    ByVal Which As System.Integer, _    ByVal Sheets As System.Object _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IExportPdfData Dim Which As System.Integer Dim Sheets As System.Object Dim value As System.Boolean   value = instance.SetSheets(Which, Sheets) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetSheets(     System.int Which,    System.object Sheets ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetSheets(  &   System.int Which, &   System.Object^ Sheets ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Which*
:   Drawing sheets to export to PDF as defined in swExportDataSheetsToExport\_e

*Sheets*
:   Array of the names of the drawing sheets to export

#### Return Value

True if the drawings sheets are set to export to PDF, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ExportPdfData::SetSheets.

# ![](dotnetimages/collapse.gif)Example

[Save File as PDF (VBA)](Save_File_as_PDF_Example_VB.htm)

[Save File as PDF (C#)](Save_File_as_PDF_Example_CSharp.htm)

[Save File as PDF (VB.NET)](Save_File_as_PDF_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IExportPdfData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExportPdfData.html)

[IExportPdfData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExportPdfData_members.html)

[IExportPdfData::GetSheets Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExportPdfData~GetSheets.html)

[IExportPdfData::GetWhichSheets Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExportPdfData~GetWhichSheets.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 SP1, Revision Number 15