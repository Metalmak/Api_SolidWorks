<!-- source: sustainabilityapi/GettingStarted-sustainabilityapi.html -->

![](images/collapse.gif)
![](images/expand.gif)
![](images/copycode.gif)
![](images/copycodeHighlight.gif)
![](images/drpdown.gif)
![](images/drpdown_orange.gif)

|  |
| --- |
|  |

|  |  |
| --- | --- |
| SOLIDWORKS Sustainability API Help |  |
| Getting Started |
| Send Feedback | |

Glossary Item Box

Writing a SOLIDWORKS Sustainability API application typically involves:

1. Adding a reference to either the SOLIDWORKS Sustainability API type library or primary interop assembly:
   * VBA: **sustainability** *version* **Type Library** or *install\_dir*\**sustainability.tlb**.* C# or VB.NET: **SOLIDWORKS.Interop.sustainability** or *install\_dir*\**api\redist\SOLIDWORKS.Interop.sustainability.dll**.
       **NOTE**: *install\_dir* is typically **C:\Program Files\SOLIDWORKS Corp\SOLIDWORKS**.- Opening a part or assembly document.- Getting the model document object, IModelDoc2.- Calling IModelDocExtension::GetSustainability to get the entry point to the SOLIDWORKS Sustainability API, [ISustainabilityApp](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityApp.html).- Getting and setting environmental impact factors:

           | For document type... | To get or set this environmental impact factor... | Call... |
           | --- | --- | --- |
           | Parts | [Material](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityMaterial.html) | [ISustainabilityApp::GetSustainabilityMaterial](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityApp~GetSustainabilityMaterial.html) |
           |  | [Manufacture](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityManufacturing.html) | [ISustainabilityApp::GetSustainabilityManufacturing](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityApp~GetSustainabilityManufacturing.html) |
           |  | [Region of use](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityUse.html) | [ISustainabilityApp::GetSustainabilityPartUse](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityApp~GetSustainabilityPartUse.html) |
           |  | [Transportation](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityTransportation.html) | [ISustainabilityApp::GetSustainabilityTransportation](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityApp~GetSustainabilityTransportation.html) |
           |  | [End of Life](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityEndOfLife.html) | [ISustainabilityApp::GetSustainabilityEndOfLife](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityApp~GetSustainabilityEndOfLife.html) |
           |  |  |  |
           | Assemblies | [Material](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityMaterial.html) of components | [ISustainabilityApp::GetSustainabilityMaterial](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityApp~GetSustainabilityMaterial.html) |
           |  | [Manufacture](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityManufacturing.html) of components | [ISustainabilityApp::GetSustainabilityManufacturing](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityApp~GetSustainabilityManufacturing.html) |
           |  | [Assembly](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityAssemblyProcess.html) | [ISustainabilityApp::GetSustainabilityAssemblyProcess](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityApp~GetSustainabilityAssemblyProcess.html) |
           |  | [Region of use and energy consumption](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityAssemblyUse.html) | [ISustainabilityApp::GetSustainabilityAssemblyUse](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityApp~GetSustainabilityAssemblyUse.html) |
           |  | [Transportation](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityTransportation.html) | [ISustainabilityApp::GetSustainabilityTransportation](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityApp~GetSustainabilityTransportation.html) |
           |  | [End of Life](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityEndOfLife.html) | [ISustainabilityApp::GetSustainabilityEndOfLife](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityApp~GetSustainabilityEndOfLife.html) |

           - Specifying the [amount of product use time](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityEnvironmentalImpact~DurationOfUse.html) over which to evaluate environmental impact.- Specifying the [units](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityEnvironmentalImpact~DurationType.html) of time over which to evaluate environmental impact.- [Updating the environmental impact results](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityEnvironmentalImpact~UpdateResults.html).- Obtaining the environmental impact of a part or assembly in terms of [air acidification](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityEnvironmentalImpact~GetAirAcidification.html), [carbon footprint](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityEnvironmentalImpact~GetCurrentCarbonFootPrint.html), [energy consumption](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityEnvironmentalImpact~GetEnergyConsumption.html), and [water eutrophication](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityEnvironmentalImpact~GetWaterEutrophication.html).

For more information about SOLIDWORKS Sustainability, see the SOLIDWORKS Help.

©2022. All Rights Reserved.