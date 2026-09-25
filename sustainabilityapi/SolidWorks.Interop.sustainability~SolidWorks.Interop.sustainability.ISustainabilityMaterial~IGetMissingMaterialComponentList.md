<!-- source: sustainabilityapi/SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial~IGetMissingMaterialComponentList.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Sustainability API Help | Send comments on this topic. |
| IGetMissingMaterialComponentList Method (ISustainabilityMaterial) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sustainability Namespace](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability_namespace.html) > [ISustainabilityMaterial Interface](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial.html) : IGetMissingMaterialComponentList Method (ISustainabilityMaterial) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Count*
:   Number of assembly components returned in ComponentsNames (see **Remarks**)

*ComponentsNames*
:   * in-process, unmanaged C++: Pointer to an array of the names of the assembly components that are missing materials* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

Gets the names of the assembly components that are missing materials.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub IGetMissingMaterialComponentList( _    ByVal Count As System.Integer, _    ByRef ComponentsNames As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISustainabilityMaterial Dim Count As System.Integer Dim ComponentsNames As System.String   instance.IGetMissingMaterialComponentList(Count, ComponentsNames) ``` | |

| C# |  |
| --- | --- |
| ``` void IGetMissingMaterialComponentList(     System.int Count,    ref System.string ComponentsNames ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void IGetMissingMaterialComponentList(  &   System.int Count, &   System.String^% ComponentsNames ) ``` | |

#### Parameters

*Count*
:   Number of assembly components returned in ComponentsNames (see **Remarks**)

*ComponentsNames*
:   * in-process, unmanaged C++: Pointer to an array of the names of the assembly components that are missing materials* VBA, VB.NET, C#, and C++/CLI: Not supported

    See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [ISustainabilityMaterial::GetMissingMaterialComponentCount](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityMaterial~GetMissingMaterialComponentCount.html) to assign Count.

# ![](dotnetimages/collapse.gif)See Also

####

[ISustainabilityMaterial Interface](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial.html)

[ISustainabilityMaterial Members](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial_members.html)

[ISustainabilityMaterial::GetMissingMaterialComponentList Method](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityMaterial~GetMissingMaterialComponentList.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Sustainability API 2013 SP0