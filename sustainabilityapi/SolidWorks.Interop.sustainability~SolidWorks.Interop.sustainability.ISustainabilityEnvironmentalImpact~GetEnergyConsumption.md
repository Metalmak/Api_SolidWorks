<!-- source: sustainabilityapi/SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityEnvironmentalImpact~GetEnergyConsumption.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Sustainability API Help | Send comments on this topic. |
| GetEnergyConsumption Method (ISustainabilityEnvironmentalImpact) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sustainability Namespace](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability_namespace.html) > [ISustainabilityEnvironmentalImpact Interface](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityEnvironmentalImpact.html) : GetEnergyConsumption Method (ISustainabilityEnvironmentalImpact) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Values*
:   Array of five doubles of megajoules of energy consumed by material, use, transportation, manufacturing, and end of life environmental impact factors

Obsolete. Superseded by [ISustainabilityEnvironmentalImpact::GetEnergyConsumption2](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityEnvironmentalImpact~GetEnergyConsumption2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetEnergyConsumption( _    ByRef Values As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISustainabilityEnvironmentalImpact Dim Values As System.Object Dim value As System.Integer   value = instance.GetEnergyConsumption(Values) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetEnergyConsumption(     out System.object Values ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetEnergyConsumption(  &   [Out] System.Object^ Values ) ``` | |

#### Parameters

*Values*
:   Array of five doubles of megajoules of energy consumed by material, use, transportation, manufacturing, and end of life environmental impact factors

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SustainabilityEnvironmentalImpact::GetEnergyConsumption.

# ![](dotnetimages/collapse.gif)Example

See the examples in [ISustainabilityEnvironmentalImpact](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityEnvironmentalImpact.html).

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call:

1. [ISustainabilityEnvironmentalImpact::DurationOfUse](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityEnvironmentalImpact~DurationOfUse.html)- [ISustainabilityEnvironmentalImpact::DurationType](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityEnvironmentalImpact~DurationType.html)- [ISustainabilityEnvironmentalImpact::UpdateResults](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityEnvironmentalImpact~UpdateResults.html)

# ![](dotnetimages/collapse.gif)See Also

####

[ISustainabilityEnvironmentalImpact Interface](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityEnvironmentalImpact.html)

[ISustainabilityEnvironmentalImpact Members](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityEnvironmentalImpact_members.html)

[ISustainabilityEnvironmentalImpact::IGetEnergyConsumption Method](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityEnvironmentalImpact~IGetEnergyConsumption.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Sustainability API 2013 SP0