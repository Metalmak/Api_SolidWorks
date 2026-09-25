<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFrequencyStudyOptions~FlowTemperatureFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| FlowTemperatureFile Property (ICWFrequencyStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWFrequencyStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFrequencyStudyOptions.html) : FlowTemperatureFile Property (ICWFrequencyStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the SOLIDWORKS Flow Simulation result file that is used to import flow temperatures.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property FlowTemperatureFile As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWFrequencyStudyOptions Dim value As System.String   instance.FlowTemperatureFile = value   value = instance.FlowTemperatureFile ``` | |

| C# |  |
| --- | --- |
| ``` System.string FlowTemperatureFile {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ FlowTemperatureFile {    System.String^ get();    void set ( &   System.String^ value); } ``` | |

#### Property Value

Full path name of a SOLIDWORKS Flow Simulation result file (**\*.fld**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWFrequencyStudyOptions::FlowTemperatureFile.

# ![](dotnetimages/collapse.gif)Example

See the [ICWFrequencyStudyOptions](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFrequencyStudyOptions.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only if [ICWFrequencyStudyOptions::ThermalResults](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFrequencyStudyOptions~ThermalResults.html) is set to [swsThermalOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsThermalOption_e.html).swsThermalOption\_TemperatureFromFlow.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWFrequencyStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFrequencyStudyOptions.html)

[ICWFrequencyStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWFrequencyStudyOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2017 SP0