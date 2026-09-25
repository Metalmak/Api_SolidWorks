<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMaterialErrorWarning_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsMaterialErrorWarning\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsMaterialErrorWarning\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Material errors

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsMaterialErrorWarning_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsMaterialErrorWarning_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsMaterialErrorWarning_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsMaterialErrorWarning_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsMaterialErrorWarningCreepWithForceControl** | 24 = Creep option for material works only with force control method; error |
| **swsMaterialErrorWarningDefineCurveForEx** | 10 = Define curve for EX; error |
| **swsMaterialErrorWarningDefinePointForStressStrainCurve** | 16 = Define point (0,0) for this stress-strain curve; error |
| **swsMaterialErrorWarningDefineProperty** | 6 = Define at least one property; error |
| **swsMaterialErrorWarningDefineStressStrainCurve** | 15 = Define stress-strain curve for material; error |
| **swsMaterialErrorWarningDensityNotDefined** | 13 = Material density not defined; error |
| **swsMaterialErrorWarningEXNotDefined** | 8 = EX (modulus of elasticity) not defined; error |
| **swsMaterialErrorWarningEXValue** | 9 =EX should be > 0; error |
| **swsMaterialErrorWarningFatigueSNCurvesCycles** | 3 = Cycle values of fatigue S-N curves should be monotonically increasing; error |
| **swsMaterialErrorWarningInvalidLinearElasticAnisotropicMaterialModel** | 1 = The linear elastic anisotropic material model is invalid for this study; error |
| **swsMaterialErrorWarningInvalidMaterialModel** | 2 = Invalid material model for this study; error |
| **swsMaterialErrorWarningMaterialPropertyValue** | 7 = Material property value should be > 0; error |
| **swsMaterialErrorWarningMaterialTemperatureCurveForNitinol** | 11 = Material temperature curve is not allowed for Nitinol; error |
| **swsMaterialErrorWarningMaterialTemperatureDependencyIgnored** | 30 = Material temperature dependency is ignored for drop test analysis; warning |
| **swsMaterialErrorWarningNUXYNotDefined** | 32 = Poisson's Ratio (NUXY) is not defined; program will use a default value of 0.0; warning |
| **swsMaterialErrorWarningNUXYValue** | 12 = NUXY (Poissons Ratio) should be < 0.5; error |
| **swsMaterialErrorWarningOnlyBilinearPlasticityForDropTestStudies** | 31 = Only bilinear plasticity is supported for drop test studies; stress-strain curves are ignored; warning |
| **swsMaterialErrorWarningrKXNotDefined** | 14 = KX (thermal conductivity) not defined; error |
| **swsMaterialErrorWarningSIGC\_F2LessThanSIGC\_S2** | 23 = Property SIGC\_F2 should be less than SIGC\_S2; error |
| **swsMaterialErrorWarningSIGC\_S1LessThanSIGC\_F1** | 21 = Property SIGC\_S1 should be less than SIGC\_F1; error |
| **swsMaterialErrorWarningSIGC\_S2LessThanSIGC\_F1** | 22 = Property SIGC\_S2 should be less than SIGC\_F1; error |
| **swsMaterialErrorWarningSIGT\_F2LessThanSIGT\_S2** | 20 = Property SIGT\_F2 should be less than SIGT\_S2; error |
| **swsMaterialErrorWarningSIGT\_S1\_F1\_S2\_F2Values** | 17 = Properties SIGT\_S1, SIGT\_F1, SIGT\_S2 and SIGT\_F2 should be > 0; error |
| **swsMaterialErrorWarningSIGT\_S1LessThanSIGT\_F1** | 18 = Property SIGT\_S1 should be less than SIGT\_F1; error |
| **swsMaterialErrorWarningSIGT\_S2LessThanSIGT\_F1** | 19 = Property SIGT\_S2 should be less than SIGT\_F1; error |
| **swsMaterialErrorWarningSuccessful** | 0 = Successful |
| **swsMaterialErrorWarningTooManyPointsSNCurve** | 5 = S-N curves should not have more than 200 data points; error |
| **swsMaterialErrorWarningUniqueStressRatioForEachSNCurve** | 4 = Stress ratio should be unique for each S-N curve; error |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)