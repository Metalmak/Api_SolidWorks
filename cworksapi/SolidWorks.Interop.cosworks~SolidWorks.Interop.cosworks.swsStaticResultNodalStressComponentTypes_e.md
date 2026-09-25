<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsStaticResultNodalStressComponentTypes_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsStaticResultNodalStressComponentTypes\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsStaticResultNodalStressComponentTypes\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Nodal stress component types for static study results

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsStaticResultNodalStressComponentTypes_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsStaticResultNodalStressComponentTypes_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsStaticResultNodalStressComponentTypes_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsStaticResultNodalStressComponentTypes_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsStaticNodalStress\_INT** | 10 = Stress intensity (P1-P3) |
| **swsStaticNodalStress\_P1** | 6 = Normal stress in the first principal direction |
| **swsStaticNodalStress\_P2** | 7 = Normal stress in the second principal direction |
| **swsStaticNodalStress\_P3** | 8 = Normal stress in the third principal direction |
| **swsStaticNodalStress\_SX** | 0 = Normal stress in the X direction of the selected reference geometry |
| **swsStaticNodalStress\_SY** | 1 = Normal stress in the Y direction of the selected reference geometry |
| **swsStaticNodalStress\_SZ** | 2 = Normal stress in the Z direction of the selected reference geometry |
| **swsStaticNodalStress\_TRI** | 11 = Triaxial stress (P1+P2+P3) |
| **swsStaticNodalStress\_TXY** | 3 = Shear stress in the Y direction on the YZ plane of the selected reference geometry |
| **swsStaticNodalStress\_TXZ** | 4 = Shear stress in the Z direction on the YZ plane of the selected reference geometry |
| **swsStaticNodalStress\_TYZ** | 5 = Shear stress in the Z direction on the XZ plane of the selected reference geometry |
| **swsStaticNodalStress\_VON** | 9 = von Mises stress |

# ![](dotnetimages/collapse.gif)Remarks

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)