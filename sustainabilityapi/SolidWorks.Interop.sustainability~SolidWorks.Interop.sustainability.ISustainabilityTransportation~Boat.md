<!-- source: sustainabilityapi/SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityTransportation~Boat.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Sustainability API Help | Send comments on this topic. |
| Boat Property (ISustainabilityTransportation) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sustainability Namespace](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability_namespace.html) > [ISustainabilityTransportation Interface](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityTransportation.html) : Boat Property (ISustainabilityTransportation) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the distance traveled by boat from the region of manufacture to the region of use.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property Boat As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISustainabilityTransportation Dim value As System.Double   instance.Boat = value   value = instance.Boat ``` | |

| C# |  |
| --- | --- |
| ``` System.double Boat {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double Boat {    System.double get();    void set ( &   System.double value); } ``` | |

#### Property Value

0.0 <= Distance in kilometers or miles traveled by boat <= 100,000,000.0

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SustainabilityTransportation::Boat.

# ![](dotnetimages/collapse.gif)Example

See the examples in [ISustainabilityTransportation](SOLIDWORKS.Interop.sustainability~SOLIDWORKS.Interop.sustainability.ISustainabilityTransportation.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ISustainabilityTransportation Interface](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityTransportation.html)

[ISustainabilityTransportation Members](SolidWorks.Interop.sustainability~SolidWorks.Interop.sustainability.ISustainabilityTransportation_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Sustainability API 2013 SP0