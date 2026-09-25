<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExportPdfData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IExportPdfData Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExportPdfData_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IExportPdfData Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to the PDF export data interface, which allows you to save:

* one or more drawing sheets to PDF.* parts and assemblies to 3D PDF.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IExportPdfData ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IExportPdfData ``` | |

| C# |  |
| --- | --- |
| ``` public interface IExportPdfData ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IExportPdfData ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ExportPdfData.

# ![](dotnetimages/collapse.gif)Example

[Save File as PDF (VBA)](Save_File_as_PDF_Example_VB.htm)

[Save File as PDF (C#)](Save_File_as_PDF_Example_CSharp.htm)

[Save File as PDF (VB.NET)](Save_File_as_PDF_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

**To export one or more drawing sheets to PDF:**

1. Get the IExportPdfData object using [ISldWorks::GetExportFileData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~GetExportFileData.html).

   - Set the sheets to export to PDF using [IExportPdfData::SetSheets](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IExportPdfData~SetSheets.html).

     - Set whether to view the PDF after saving using [IExportPdfData::ViewPdfAfterSaving](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IExportPdfData~ViewPdfAfterSaving.html).

       - Save the sheets using [IModelDocExtension::SaveAs](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SaveAs.html).

**To export a part or assembly to 3D PDF:**

1. Get the IExportPdfData object using [ISldWorks::GetExportFileData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~GetExportFileData.html).

   - Set [IExportPdfData::ExportAs3D](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IExportPdfData~ExportAs3D.html) to true.

     - Set whether to view the PDF after saving using [IExportPdfData::ViewPdfAfterSaving](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IExportPdfData~ViewPdfAfterSaving.html).

       - Save the part or assembly using [IModelDocExtension::SaveAs](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SaveAs.html).

# ![](dotnetimages/collapse.gif)Accessors

[ISldWorks::GetExportFileData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~GetExportFileData.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[ExportPdfData](SWObjectModel.pdf#ExportPdfData)

# ![](dotnetimages/collapse.gif)See Also

####

[IExportPdfData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IExportPdfData_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)