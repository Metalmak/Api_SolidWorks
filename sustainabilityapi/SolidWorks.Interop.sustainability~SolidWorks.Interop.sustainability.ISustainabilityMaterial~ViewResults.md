<!-- source: sustainabilityapi/SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial~ViewResults.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Sustainability API Help | Send comments on this topic. |
| ViewResults Method (ISustainabilityMaterial) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sustainability Namespace](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability_namespace.html) > [ISustainabilityMaterial Interface](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial.html) : ViewResults Method (ISustainabilityMaterial) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Switches the Sustainability Task Pane from Task List to Assembly Process and calculates the environmental impact of assemblies only.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ViewResults() ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISustainabilityMaterial   instance.ViewResults() ``` | |

| C# |  |
| --- | --- |
| ``` void ViewResults() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ViewResults(); ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SustainabilityMaterial::ViewResults.

# ![](dotnetimages/collapse.gif)Example

[Calculate Environmental Impact of Assembly (VBA)](Calculate_Environmental_Impact_of_Assembly_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

| Before calling this method, call... | To... |
| --- | --- |
| [ISustainabilityMaterial::ExcludeComponent](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityMaterial~ExcludeComponent.html) or [ISustainabilityMaterial::IExcludeComponent](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityMaterial~IExcludeComponent.html) | Exclude components from the environmental impact calculation |
| [ISustainabilityMaterial::IncludeComponent](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityMaterial~IncludeComponent.html) or [ISustainabilityMaterial::IIncludeComponent](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityMaterial~IIncludeComponent.html) | Include components that were previously excluded from the environmental impact calculation |
| [ISustainabilityMaterial::GetMissingMaterialComponentList](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityMaterial~GetMissingMaterialComponentList.html) or [ISustainabilityMaterial::IGetMissingMaterialComponentList](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityMaterial~IGetMissingMaterialComponentList.html) | Get the names of the components that are missing materials |
| [ISustainabilityMaterial::MaterialClass](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityMaterial~MaterialClass.html) | Specify the material class |
| [ISustainabilityMaterial::MaterialName](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityMaterial~MaterialName.html) | Specify the material name |
| [ISustainabilityMaterial::SetPropertiesForComponent](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityMaterial~SetPropertiesForComponent.html) or [ISustainabilityMaterial::ISetPropertiesForComponent](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityMaterial~ISetPropertiesForComponent.html) | Set the specified material for the specified components |

# ![](dotnetimages/collapse.gif)See Also

####

[ISustainabilityMaterial Interface](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial.html)

[ISustainabilityMaterial Members](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0