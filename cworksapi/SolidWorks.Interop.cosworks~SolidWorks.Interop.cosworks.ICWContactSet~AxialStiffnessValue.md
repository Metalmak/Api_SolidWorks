<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactSet~AxialStiffnessValue.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| AxialStiffnessValue Property (ICWContactSet) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWContactSet Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactSet.html) : AxialStiffnessValue Property (ICWContactSet) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the wall axial stiffness value for this flexible virtual wall contact set.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property AxialStiffnessValue As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWContactSet Dim value As System.Double   instance.AxialStiffnessValue = value   value = instance.AxialStiffnessValue ``` | |

| C# |  |
| --- | --- |
| ``` System.double AxialStiffnessValue {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.double AxialStiffnessValue {    System.double get();    void set ( &   System.double value); } ``` | |

#### Property Value

Wall axial stiffness value

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWContactSet::AxialStiffnessValue.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only if [ICWContactSet::ContactSetType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactSet~ContactSetType.html) is set to [swsContactSetTypeStaticNonLinear\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsContactSetTypeStaticNonLinear_e.html).swsContactSetTypeStaticNonLinearVirtualWall and [ICWContactSet::WallType](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactSet~WallType.html) is set to [swsWallType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsWallType_e.html).swsWallTypeFlexible.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWContactSet Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactSet.html)

[ICWContactSet Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactSet_members.html)

[ICWContactSet::WallStiffnessUnit Property ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWContactSet~WallStiffnessUnit.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0