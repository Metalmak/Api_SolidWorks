<!-- source: sustainabilityapi/SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityAssemblyProcess~AssemblyProcessAmount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Sustainability API Help | Send comments on this topic. |
| AssemblyProcessAmount Property (ISustainabilityAssemblyProcess) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sustainability Namespace](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability_namespace.html) > [ISustainabilityAssemblyProcess Interface](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityAssemblyProcess.html) : AssemblyProcessAmount Property (ISustainabilityAssemblyProcess) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the amount of fuel required to assemble this assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property AssemblyProcessAmount As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISustainabilityAssemblyProcess Dim value As System.Object   instance.AssemblyProcessAmount = value   value = instance.AssemblyProcessAmount ``` | |

| C# |  |
| --- | --- |
| ``` System.object AssemblyProcessAmount {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.Object^ AssemblyProcessAmount {    System.Object^ get();    void set ( &   System.Object^ value); } ``` | |

#### Property Value

Array containing the amounts of electricity and natural gas required to assemble this assembly; valid only if [ISustainabilityAssemblyProcess::EnergyForAssemblyProcess](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityAssemblyProcess~EnergyForAssemblyProcess.html) is true

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SustainabilityAssemblyProcess::AssemblyProcessAmount.

# ![](dotnetimages/collapse.gif)Example

See the examples in [ISustainabilityAssemblyProcess](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityAssemblyProcess.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISustainabilityAssemblyProcess Interface](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityAssemblyProcess.html)

[ISustainabilityAssemblyProcess Members](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityAssemblyProcess_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Sustainability API 2013 SP0