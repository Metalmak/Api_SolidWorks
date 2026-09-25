<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~ExportSimulationStudy.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ExportSimulationStudy Method (ICWStudy) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html) : ExportSimulationStudy Method (ICWStudy) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SLocationPath*
:   Path to which to export this study

*SFileName*
:   Name of file to which to export this study

*NFormat*
:   | If nOption is swsStudyExportOption\_e... | nFormat is... |
    | --- | --- |
    | swsStudyExport\_Cosmos | Export option as defined by [swsCosmosExportOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsCosmosExportOption_e.html) |
    | swsStudyExport\_Nastran | Format in which to export this study as defined by [swsNastranExportOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsNastranExportOption_e.html) |
    | swsStudyExport\_Abacus, swsStudyExport\_Ansys, swsStudyExport\_Exodus, swsStudyExport\_IdeasUniversal, or swsStudyExport\_PatranNeutral | Not valid |

*NNodeOffset*
:   Starting node for exported data; the lowest node label in the generated file is NNodeOffset + 1

*NElementOffset*
:   Starting element for exported data; the lowest element label in the generated file is NElementOffset + 1

*NOption*
:   Finite-element analysis program to which to export as defined by [swsStudyExportOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStudyExportOption_e.html)

*NUnit*
:   | If nOption is swsStudyExportOption\_e... | nUnit is... |
    | --- | --- |
    | swsStudyExport\_Cosmos | Defined by [swsLinearUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLinearUnit_e.html) |
    | swsStudyExport\_Nastran | Defined by [swsNastranExportUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsNastranExportUnit_e.html) |
    | swsStudyExport\_Abacus, swsStudyExport\_Ansys, swsStudyExport\_Exodus, swsStudyExport\_IdeasUniversal, or swsStudyExport\_PatranNeutral | Not valid |

Exports this study to the specified finite-element analysis program.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ExportSimulationStudy( _    ByVal SLocationPath As System.String, _    ByVal SFileName As System.String, _    ByVal NFormat As System.Integer, _    ByVal NNodeOffset As System.Integer, _    ByVal NElementOffset As System.Integer, _    ByVal NOption As System.Integer, _    ByVal NUnit As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudy Dim SLocationPath As System.String Dim SFileName As System.String Dim NFormat As System.Integer Dim NNodeOffset As System.Integer Dim NElementOffset As System.Integer Dim NOption As System.Integer Dim NUnit As System.Integer Dim value As System.Integer   value = instance.ExportSimulationStudy(SLocationPath, SFileName, NFormat, NNodeOffset, NElementOffset, NOption, NUnit) ``` | |

| C# |  |
| --- | --- |
| ``` System.int ExportSimulationStudy(     System.string SLocationPath,    System.string SFileName,    System.int NFormat,    System.int NNodeOffset,    System.int NElementOffset,    System.int NOption,    System.int NUnit ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ExportSimulationStudy(  &   System.String^ SLocationPath, &   System.String^ SFileName, &   System.int NFormat, &   System.int NNodeOffset, &   System.int NElementOffset, &   System.int NOption, &   System.int NUnit ) ``` | |

#### Parameters

*SLocationPath*
:   Path to which to export this study

*SFileName*
:   Name of file to which to export this study

*NFormat*
:   | If nOption is swsStudyExportOption\_e... | nFormat is... |
    | --- | --- |
    | swsStudyExport\_Cosmos | Export option as defined by [swsCosmosExportOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsCosmosExportOption_e.html) |
    | swsStudyExport\_Nastran | Format in which to export this study as defined by [swsNastranExportOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsNastranExportOption_e.html) |
    | swsStudyExport\_Abacus, swsStudyExport\_Ansys, swsStudyExport\_Exodus, swsStudyExport\_IdeasUniversal, or swsStudyExport\_PatranNeutral | Not valid |

*NNodeOffset*
:   Starting node for exported data; the lowest node label in the generated file is NNodeOffset + 1

*NElementOffset*
:   Starting element for exported data; the lowest element label in the generated file is NElementOffset + 1

*NOption*
:   Finite-element analysis program to which to export as defined by [swsStudyExportOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStudyExportOption_e.html)

*NUnit*
:   | If nOption is swsStudyExportOption\_e... | nUnit is... |
    | --- | --- |
    | swsStudyExport\_Cosmos | Defined by [swsLinearUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsLinearUnit_e.html) |
    | swsStudyExport\_Nastran | Defined by [swsNastranExportUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsNastranExportUnit_e.html) |
    | swsStudyExport\_Abacus, swsStudyExport\_Ansys, swsStudyExport\_Exodus, swsStudyExport\_IdeasUniversal, or swsStudyExport\_PatranNeutral | Not valid |

#### Return Value

Error as defined in [swsStudyExportError\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsStudyExportError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudy::ExportSimulationStudy.

# ![](dotnetimages/collapse.gif)Example

[Apply Thermostat-controlled Heat Power for Transient Thermal Study (VBA)](Apply_Thermostat-controlled_Heat_Power_for_Transient_Thermal_Study_Example_VB.htm)

[Apply Thermostat-controlled Heat Power for Transient Thermal Study (VB.NET)](Apply_Thermostat-controlled_Heat_Power_for_Transient_Thermal_Study_Example_VBNET.htm)

[Apply Thermostat-controlled Heat Power for Transient Thermal Study (C#)](Apply_Thermostat-controlled_Heat_Power_for_Transient_Thermal_Study_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html)

[ICWStudy Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy_members.html)

[ICWStudy::GenerateReport Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~GenerateReport.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2014 SP0