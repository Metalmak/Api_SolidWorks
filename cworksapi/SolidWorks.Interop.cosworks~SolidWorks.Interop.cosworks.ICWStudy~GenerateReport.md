<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~GenerateReport.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GenerateReport Method (ICWStudy) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html) : GenerateReport Method (ICWStudy) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SReportPath*
:   Path in which to create this report

*SDocName*
:   File name of the report

*BShowOnPublish*
:   True to display the report after creation, false to not

Creates a report about all aspects of this study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GenerateReport( _    ByVal SReportPath As System.String, _    ByVal SDocName As System.String, _    ByVal BShowOnPublish As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudy Dim SReportPath As System.String Dim SDocName As System.String Dim BShowOnPublish As System.Boolean Dim value As System.Integer   value = instance.GenerateReport(SReportPath, SDocName, BShowOnPublish) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GenerateReport(     System.string SReportPath,    System.string SDocName,    System.bool BShowOnPublish ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GenerateReport(  &   System.String^ SReportPath, &   System.String^ SDocName, &   System.bool BShowOnPublish ) ``` | |

#### Parameters

*SReportPath*
:   Path in which to create this report

*SDocName*
:   File name of the report

*BShowOnPublish*
:   True to display the report after creation, false to not

#### Return Value

Error code as defined in [swsGenerateReportError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsGenerateReportError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudy::GenerateReport.

# ![](dotnetimages/collapse.gif)Example

[Copy Mesh and Generate Report (VBA)](Copy_Mesh_and_Gen_Report_Example_VB.htm)

[Copy Mesh and Generate Report (VB.NET)](Copy_Mesh_and_Gen_Report_Example_VBNET.htm)

[Copy Mesh and Generate Report (C#)](Copy_Mesh_and_Gen_Report_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html)

[ICWStudy Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy_members.html)

[ICWStudy::ExportSimulationStudy Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~ExportSimulationStudy.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0