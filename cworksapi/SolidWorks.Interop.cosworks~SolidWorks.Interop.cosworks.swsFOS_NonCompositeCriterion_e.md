<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFOS_NonCompositeCriterion_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsFOS\_NonCompositeCriterion\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsFOS\_NonCompositeCriterion\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Factor of safety criteria for non-composite shells

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsFOS_NonCompositeCriterion_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsFOS_NonCompositeCriterion_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsFOS_NonCompositeCriterion_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsFOS_NonCompositeCriterion_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsFOSNonCompositeCriterion\_Automatic** | 4 = See **Remarks** |
| **swsFOSNonCompositeCriterion\_Coulomb** | 3 = Max Normal Stress |
| **swsFOSNonCompositeCriterion\_MohrCoulomb** | 2 = Mohr-Coulomb Stress |
| **swsFOSNonCompositeCriterion\_Tresca** | 1 = Maximum Shear Stress |
| **swsFOSNonCompositeCriterion\_VonMisesHencky** | 0 = Maximum von Mises Stress |

# ![](dotnetimages/collapse.gif)Remarks

If you set swsFOSNonCompositeCriterion\_Automatic, SOLIDWORKS Simulation selects the most appropriate failure criterion across all element types by applying the following conditions:

* The default Failure Criterion assigned in the Material dialog box for each material. * If you have not assigned a default failure criterion in the Material dialog box, the software assigns the Mohr-Coulomb stress criterion. * If you selected Max von Mises or Max shear (Tresca) criterion for a beam material, the software uses the yield strength as allowable stress. * If you selected Max normal or Mohr-Coulomb criterion for a beam material, the software uses the tensile strength as the allowable stress.* For composite shells, the Tsai-Hill failure criterion is applied. * Failure indices for the composite shells failure criteria (Tsai-Hill, Tsai-Wu, and Maximum Stress) are calculated from nodal stresses.* For beams, the factor of safety is calculated from: Upper bound axial and bending stress / Yield Strength.* For assemblies, the factor of safety is calculated from the un-averaged values of stress components.

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)