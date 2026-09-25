<!-- source: sustainabilityapi/SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial~IExcludeComponent.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Sustainability API Help | Send comments on this topic. |
| IExcludeComponent Method (ISustainabilityMaterial) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sustainability Namespace](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability_namespace.html) > [ISustainabilityMaterial Interface](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial.html) : IExcludeComponent Method (ISustainabilityMaterial) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Count*
:   Number of assembly components in ExcludeComponentNames

*ExcludeComponentNames*
:   * in-process, unmanaged C++: Pointer to an array of the names of the assembly components to exclude from the calculation of environmental impact* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

Excludes the specified assembly components from the calculation of environmental impact.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IExcludeComponent( _    ByVal Count As System.Integer, _    ByRef ExcludeComponentNames As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISustainabilityMaterial Dim Count As System.Integer Dim ExcludeComponentNames As System.String   instance.IExcludeComponent(Count, ExcludeComponentNames) ``` | |

| C# |  |
| --- | --- |
| ``` void IExcludeComponent(     System.int Count,    ref System.string ExcludeComponentNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IExcludeComponent(  &   System.int Count, &   System.String^% ExcludeComponentNames ) ``` | |

#### Parameters

*Count*
:   Number of assembly components in ExcludeComponentNames

*ExcludeComponentNames*
:   * in-process, unmanaged C++: Pointer to an array of the names of the assembly components to exclude from the calculation of environmental impact* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)See Also

####

[ISustainabilityMaterial Interface](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial.html)

[ISustainabilityMaterial Members](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial_members.html)

[ISustainabilityMaterial::ExcludeComponent Method](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial~ExcludeComponent.html)

[ISustainabilityMaterial::IIncludeComponent Method](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial~IIncludeComponent.html)

[ISustainabilityMaterial::IncludeComponent Method](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial~IncludeComponent.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Sustainability API 2013 SP0