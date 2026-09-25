<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDistributedMass~Units.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| Units Property (ICWDistributedMass) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDistributedMass Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDistributedMass.html) : Units Property (ICWDistributedMass) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the units of the distributed mass.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property Units As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDistributedMass Dim value As System.Integer   instance.Units = value   value = instance.Units ``` | |

| C# |  |
| --- | --- |
| ``` System.int Units {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int Units {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

Units as defined by [swsUnitSystem\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUnitSystem_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWDistributedMass::Units.

# ![](dotnetimages/collapse.gif)Example

[Create Linear Dynamic Study (VBA)](Create_Dynamic_Harmonic_Study_Example_VB.htm)

[Create Linear Dynamic Study (VB.NET)](Create_Dynamic_Harmonic_Study_Example_VBNET.htm)

[Create Linear Dynamic Study (C#)](Create_Dynamic_Harmonic_Study_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDistributedMass Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDistributedMass.html)

[ICWDistributedMass Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDistributedMass_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0