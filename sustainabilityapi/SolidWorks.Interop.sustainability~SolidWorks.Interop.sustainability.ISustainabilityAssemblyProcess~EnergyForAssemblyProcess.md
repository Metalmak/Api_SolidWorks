<!-- source: sustainabilityapi/SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityAssemblyProcess~EnergyForAssemblyProcess.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Sustainability API Help | Send comments on this topic. |
| EnergyForAssemblyProcess Property (ISustainabilityAssemblyProcess) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sustainability Namespace](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability_namespace.html) > [ISustainabilityAssemblyProcess Interface](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityAssemblyProcess.html) : EnergyForAssemblyProcess Property (ISustainabilityAssemblyProcess) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether energy is required to create this assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property EnergyForAssemblyProcess As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISustainabilityAssemblyProcess Dim value As System.Boolean   instance.EnergyForAssemblyProcess = value   value = instance.EnergyForAssemblyProcess ``` | |

| C# |  |
| --- | --- |
| ``` System.bool EnergyForAssemblyProcess {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool EnergyForAssemblyProcess {    System.bool get();    void set ( &   System.bool value); } ``` | |

#### Property Value

True if energy is required to create this assembly, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SustainabilityAssemblyProcess::EnergyForAssemblyProcess.

# ![](dotnetimages/collapse.gif)Example

See the examples in [ISustainabilityAssemblyProcess](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityAssemblyProcess.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISustainabilityAssemblyProcess Interface](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityAssemblyProcess.html)

[ISustainabilityAssemblyProcess Members](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityAssemblyProcess_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Sustainability API 2013 SP0