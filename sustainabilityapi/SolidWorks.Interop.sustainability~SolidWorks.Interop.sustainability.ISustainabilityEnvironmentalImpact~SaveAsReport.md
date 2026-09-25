<!-- source: sustainabilityapi/SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityEnvironmentalImpact~SaveAsReport.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Sustainability API Help | Send comments on this topic. |
| SaveAsReport Method (ISustainabilityEnvironmentalImpact) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sustainability Namespace](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability_namespace.html) > [ISustainabilityEnvironmentalImpact Interface](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityEnvironmentalImpact.html) : SaveAsReport Method (ISustainabilityEnvironmentalImpact) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileType*
:   Type of FileName as defined in [swSustainabilitySaveAsFileType\_e](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.swSustainabilitySaveAsFileType_e.html)

*FileName*
:   Base name of the file to save

*SaveTo*
:   Path to FileName

Saves the environmental impact results to a file of the specified type with the specified name on the specified path.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SaveAsReport( _    ByVal FileType As System.Integer, _    ByVal FileName As System.String, _    ByVal SaveTo As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISustainabilityEnvironmentalImpact Dim FileType As System.Integer Dim FileName As System.String Dim SaveTo As System.String   instance.SaveAsReport(FileType, FileName, SaveTo) ``` | |

| C# |  |
| --- | --- |
| ``` void SaveAsReport(     System.int FileType,    System.string FileName,    System.string SaveTo ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SaveAsReport(  &   System.int FileType, &   System.String^ FileName, &   System.String^ SaveTo ) ``` | |

#### Parameters

*FileType*
:   Type of FileName as defined in [swSustainabilitySaveAsFileType\_e](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.swSustainabilitySaveAsFileType_e.html)

*FileName*
:   Base name of the file to save

*SaveTo*
:   Path to FileName

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SustainabilityEnvironmentalImpact::SaveAsReport.

# ![](dotnetimages/collapse.gif)Example

See the examples in [ISustainabilityEnvironmentalImpact](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityEnvironmentalImpact.html).

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call:

1. [ISustainabilityEnvironmentalImpact::DurationOfUse](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityEnvironmentalImpact~DurationOfUse.html)- [ISustainabilityEnvironmentalImpact::DurationType](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityEnvironmentalImpact~DurationType.html)- [ISustainabilityEnvironmentalImpact::UpdateResults](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityEnvironmentalImpact~UpdateResults.html)

# ![](dotnetimages/collapse.gif)See Also

####

[ISustainabilityEnvironmentalImpact Interface](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityEnvironmentalImpact.html)

[ISustainabilityEnvironmentalImpact Members](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityEnvironmentalImpact_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Sustainability API 2013 SP0