<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~GetPlanarMappingUVDirection.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetPlanarMappingUVDirection Method (ICWCompositeShellOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWCompositeShellOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions.html) : GetPlanarMappingUVDirection Method (ICWCompositeShellOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*DUVDir*
:   Reference plane used to calculate ply angle direction:

    * XY plane* ZX plane* YZ plane* Current view* Face or edge

Gets the reference plane used to calculate the ply angle direction.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetPlanarMappingUVDirection( _    ByRef DUVDir As System.Object _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWCompositeShellOptions Dim DUVDir As System.Object Dim value As System.Integer   value = instance.GetPlanarMappingUVDirection(DUVDir) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetPlanarMappingUVDirection(     out System.object DUVDir ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetPlanarMappingUVDirection(  &   [Out] System.Object^ DUVDir ) ``` | |

#### Parameters

*DUVDir*
:   Reference plane used to calculate ply angle direction:

    * XY plane* ZX plane* YZ plane* Current view* Face or edge

#### Return Value

Error code as defined in [swsCompositeShellOptionsError\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCompositeShellOptionsError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWCompositeShellOptions::GetPlanarMappingUVDirection.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWCompositeShellOptions::MappingType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~MappingType.html) is set to [swsCompositeShellOptionsMappingType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsCompositeShellOptionsMappingType_e.html).swsCompositeShellOptionsPlanarMapping.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWCompositeShellOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions.html)

[ICWCompositeShellOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions_members.html)

[ICWCompositeShellOptions::SetPlanarMappingUVDirection Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWCompositeShellOptions~SetPlanarMappingUVDirection.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP3