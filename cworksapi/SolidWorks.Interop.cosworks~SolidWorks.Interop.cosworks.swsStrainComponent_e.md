<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsStrainComponent_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsStrainComponent\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsStrainComponent\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Strain components

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsStrainComponent_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsStrainComponent_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsStrainComponent_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsStrainComponent_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsStrainComponentE1** | 9 = Normal strain in the first principal direction |
| **swsStrainComponentE2** | 10 = Normal strain in the second principal direction |
| **swsStrainComponentE3** | 11 = Normal strain in the third principal direction |
| **swsStrainComponentENERGY** | 8 = Total strain energy |
| **swsStrainComponentEPSX** | 0 = Normal strain in the X direction of the selected reference geometry |
| **swsStrainComponentEPSY** | 1 = Normal strain in the Y direction of the selected reference geometry |
| **swsStrainComponentEPSZ** | 2 = Normal strain in the Z direction of the selected reference geometry |
| **swsStrainComponentESTRN** | 6 = Equivalent strain |
| **swsStrainComponentGMXY** | 3 = Shear strain in the Y direction in the YZ plane of the selected reference geometry |
| **swsStrainComponentGMXZ** | 4 = Shear strain in the Z direction in the YZ plane of the selected reference geometry |
| **swsStrainComponentGMYZ** | 5 = Shear strain in the Z direction in the XZ plane of the selected reference geometry |
| **swsStrainComponentSEDENS** | 7 = Strain energy density |

# ![](dotnetimages/collapse.gif)Remarks

X, Y, Z directions correspond to the reference geometry. The first plane that appears in the FeatureManager design tree is used as the default reference geometry.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)