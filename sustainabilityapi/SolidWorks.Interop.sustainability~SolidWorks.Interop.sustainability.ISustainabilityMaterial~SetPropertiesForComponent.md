<!-- source: sustainabilityapi/SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial~SetPropertiesForComponent.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Sustainability API Help | Send comments on this topic. |
| SetPropertiesForComponent Method (ISustainabilityMaterial) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sustainability Namespace](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability_namespace.html) > [ISustainabilityMaterial Interface](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial.html) : SetPropertiesForComponent Method (ISustainabilityMaterial) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ComponentsNames*
:   Array of the names of the components to which to apply material properties

Applies material to the specified components.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetPropertiesForComponent( _    ByRef ComponentsNames As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISustainabilityMaterial Dim ComponentsNames As System.Object   instance.SetPropertiesForComponent(ComponentsNames) ``` | |

| C# |  |
| --- | --- |
| ``` void SetPropertiesForComponent(     ref System.object ComponentsNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetPropertiesForComponent(  &   System.Object^% ComponentsNames ) ``` | |

#### Parameters

*ComponentsNames*
:   Array of the names of the components to which to apply material properties

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SustainabilityMaterial::SetPropertiesForComponent.

# ![](dotnetimages/collapse.gif)Example

[Calculate Environmental Impact of Assembly (VBA)](Calculate_Environmental_Impact_of_Assembly_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [ISustainabilityMaterial::GetMissingMaterialComponentList](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityMaterial~GetMissingMaterialComponentList.html) to populate ComponentsNames with the list of all of the components that are missing material.

This method applies the following material properties to the components specified in ComponentsNames:

* [ISustainabilityMaterial::MaterialClass](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityMaterial~MaterialClass.html)* [ISustainabilityMaterial::MaterialName](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityMaterial~MaterialName.html)* [ISustainabilityMaterial::RecycledContent](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityMaterial~RecycledContent.html)

# ![](dotnetimages/collapse.gif)See Also

####

[ISustainabilityMaterial Interface](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial.html)

[ISustainabilityMaterial Members](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial_members.html)

[ISustainabilityMaterial::ISetPropertiesForComponent Method](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial~ISetPropertiesForComponent.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Sustainability API 2013 SP0