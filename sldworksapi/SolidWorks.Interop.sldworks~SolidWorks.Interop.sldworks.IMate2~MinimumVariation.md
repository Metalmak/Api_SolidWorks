<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~MinimumVariation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| MinimumVariation Property (IMate2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMate2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2.html) : MinimumVariation Property (IMate2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the minimum variation, in meters or radians, for the dimension of this distance or angle mate.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property MinimumVariation As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMate2 Dim value As System.Double   value = instance.MinimumVariation ``` | |

| C# |  |
| --- | --- |
| ``` System.double MinimumVariation {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double MinimumVariation {    System.double get(); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Minimum variation for the dimension of this mate

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Mate2::MinimumVariation.

# ![](dotnetimages/collapse.gif)Example

[Edit Mate (VBA)](Edit_Mate_Example_VB.htm)

[Get Mate Definition (VBA)](Get_Mate_Definition_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only for [IMate2::Type](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMate2~Type.html):

* swMateType\_e.swMateANGLE

   - or -

* swMateType\_e.swMateDISTANCE

For distance and angle mates:

*Minimum\_variation* =  *minimum\_value - dimension\_value*

# ![](dotnetimages/collapse.gif)See Also

####

[IMate2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2.html)

[IMate2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2_members.html)

[IMate2::DisplayDimension2 Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~DisplayDimension2.html)

[IMate2::MaximumVariation Property](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~MaximumVariation.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0