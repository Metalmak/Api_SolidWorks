<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxFactorOfSafetyWithDetailSettings2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetMinMaxFactorOfSafetyWithDetailSettings2 Method (ICWResults) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetMinMaxFactorOfSafetyWithDetailSettings2 Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BAllBodies*
:   True to use all bodies to plot the factor of safety, false to use specific bodies

*ArraySelectedEntities*
:   Array of bodies for which to plot the factor of safety; valid only if BAllBodies is set to false

*NComponent*
:   Failure criterion as defined by [swsFOS\_NonCompositeCriterion\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFOS_NonCompositeCriterion_e.html) (see **Remarks**)

*BUpperLimit*
:   True to set an upper limit, false to not

*DUpperValue*
:   Upper limit; valid only if BUpperLimit is true

*NStressUnit*
:   Units of stress as defined in [swsStrengthUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsStrengthUnit_e.html)

*NStressLimitOption*
:   Limit stress types as defined in [swsFactorOfSafetyStressLimitOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFactorOfSafetyStressLimitOption_e.html) (see **Remarks**)

*DStressValue*
:   Stress value; valid only if NStressLimitOption is swsFactorOfSafetyStressLimitOption\_e.swsFactorOfSafetyStressLimitOption\_UserDefined

*NCompressiveStressLimitOption*
:   Compressive stress limit as defined in swsFactorOfSafetyStressLimitOption\_e (see **Remarks**)

*DCompressiveStressValue*
:   Compressive stress value; valid only if NCompressiveStressLimitOption is swsFactorOfSafetyStressLimitOption\_e.swsFactorOfSafetyStressLimitOption\_UserDefined

*DMultiplicationFactor*
:   Stress limit multiplication factor

*DCompressiveStressMultiplicationFactor*
:   Compressive stress limit multiplication factor

*BCombinedStressOnBeams*
:   True to combine stress on beams, false to not

*NShellOptions*
:   Shell face on which to perform the factor of safety as defined by [swsFOS\_ShellFaceOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFOS_ShellFaceOption_e.html)

*NStepNumber*
:   Plot step number or 0; 0 gets step 1 for linear static studies and the last available plot step for nonlinear static studies

*ErrorCode*
:   Error code as defined by [swsFosPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFosPlotErrorCode_e.html)

Gets the algebraic minimum and maximum factors of safety (FOS) for non-composite shells and the specified detail settings.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetMinMaxFactorOfSafetyWithDetailSettings2( _    ByVal BAllBodies As System.Boolean, _    ByVal ArraySelectedEntities As System.Object, _    ByVal NComponent As System.Integer, _    ByVal BUpperLimit As System.Boolean, _    ByVal DUpperValue As System.Double, _    ByVal NStressUnit As System.Integer, _    ByVal NStressLimitOption As System.Integer, _    ByVal DStressValue As System.Double, _    ByVal NCompressiveStressLimitOption As System.Integer, _    ByVal DCompressiveStressValue As System.Double, _    ByVal DMultiplicationFactor As System.Double, _    ByVal DCompressiveStressMultiplicationFactor As System.Double, _    ByVal BCombinedStressOnBeams As System.Boolean, _    ByVal NShellOptions As System.Integer, _    ByVal NStepNumber As System.Integer, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim BAllBodies As System.Boolean Dim ArraySelectedEntities As System.Object Dim NComponent As System.Integer Dim BUpperLimit As System.Boolean Dim DUpperValue As System.Double Dim NStressUnit As System.Integer Dim NStressLimitOption As System.Integer Dim DStressValue As System.Double Dim NCompressiveStressLimitOption As System.Integer Dim DCompressiveStressValue As System.Double Dim DMultiplicationFactor As System.Double Dim DCompressiveStressMultiplicationFactor As System.Double Dim BCombinedStressOnBeams As System.Boolean Dim NShellOptions As System.Integer Dim NStepNumber As System.Integer Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetMinMaxFactorOfSafetyWithDetailSettings2(BAllBodies, ArraySelectedEntities, NComponent, BUpperLimit, DUpperValue, NStressUnit, NStressLimitOption, DStressValue, NCompressiveStressLimitOption, DCompressiveStressValue, DMultiplicationFactor, DCompressiveStressMultiplicationFactor, BCombinedStressOnBeams, NShellOptions, NStepNumber, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetMinMaxFactorOfSafetyWithDetailSettings2(     System.bool BAllBodies,    System.object ArraySelectedEntities,    System.int NComponent,    System.bool BUpperLimit,    System.double DUpperValue,    System.int NStressUnit,    System.int NStressLimitOption,    System.double DStressValue,    System.int NCompressiveStressLimitOption,    System.double DCompressiveStressValue,    System.double DMultiplicationFactor,    System.double DCompressiveStressMultiplicationFactor,    System.bool BCombinedStressOnBeams,    System.int NShellOptions,    System.int NStepNumber,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetMinMaxFactorOfSafetyWithDetailSettings2(  &   System.bool BAllBodies, &   System.Object^ ArraySelectedEntities, &   System.int NComponent, &   System.bool BUpperLimit, &   System.double DUpperValue, &   System.int NStressUnit, &   System.int NStressLimitOption, &   System.double DStressValue, &   System.int NCompressiveStressLimitOption, &   System.double DCompressiveStressValue, &   System.double DMultiplicationFactor, &   System.double DCompressiveStressMultiplicationFactor, &   System.bool BCombinedStressOnBeams, &   System.int NShellOptions, &   System.int NStepNumber, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*BAllBodies*
:   True to use all bodies to plot the factor of safety, false to use specific bodies

*ArraySelectedEntities*
:   Array of bodies for which to plot the factor of safety; valid only if BAllBodies is set to false

*NComponent*
:   Failure criterion as defined by [swsFOS\_NonCompositeCriterion\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFOS_NonCompositeCriterion_e.html) (see **Remarks**)

*BUpperLimit*
:   True to set an upper limit, false to not

*DUpperValue*
:   Upper limit; valid only if BUpperLimit is true

*NStressUnit*
:   Units of stress as defined in [swsStrengthUnit\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsStrengthUnit_e.html)

*NStressLimitOption*
:   Limit stress types as defined in [swsFactorOfSafetyStressLimitOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFactorOfSafetyStressLimitOption_e.html) (see **Remarks**)

*DStressValue*
:   Stress value; valid only if NStressLimitOption is swsFactorOfSafetyStressLimitOption\_e.swsFactorOfSafetyStressLimitOption\_UserDefined

*NCompressiveStressLimitOption*
:   Compressive stress limit as defined in swsFactorOfSafetyStressLimitOption\_e (see **Remarks**)

*DCompressiveStressValue*
:   Compressive stress value; valid only if NCompressiveStressLimitOption is swsFactorOfSafetyStressLimitOption\_e.swsFactorOfSafetyStressLimitOption\_UserDefined

*DMultiplicationFactor*
:   Stress limit multiplication factor

*DCompressiveStressMultiplicationFactor*
:   Compressive stress limit multiplication factor

*BCombinedStressOnBeams*
:   True to combine stress on beams, false to not

*NShellOptions*
:   Shell face on which to perform the factor of safety as defined by [swsFOS\_ShellFaceOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFOS_ShellFaceOption_e.html)

*NStepNumber*
:   Plot step number or 0; 0 gets step 1 for linear static studies and the last available plot step for nonlinear static studies

*ErrorCode*
:   Error code as defined by [swsFosPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFosPlotErrorCode_e.html)

#### Return Value

Array of two doubles of the minimum and maximum factors of safety

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetMinMaxFactorOfSafetyWithDetailSettings2.

# ![](dotnetimages/collapse.gif)Example

[Get Factor of Safety Values (VBA)](Get_Factor_of_Safety_Values_for_Composites_Example_VB.htm)

[Get Factor of Safety Values (VB.NET)](Get_Factor_of_Safety_Values_for_Composites_Example_VBNET.htm)

[Get Factor of Safety Values (C#)](Get_Factor_of_Safety_Values_for_Composites_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If nonlinearities exist in the study, be advised to not use Factor of Safety to estimate the load-bearing capacity of the system.

| For... | Specify NComponent with swsFOS\_NonCompositeCriterion\_e.... |
| --- | --- |
| Ductile materials | * swsFOSNonCompositeCriterion\_VonMisesHencky      - or -   * swsFOSNonCompositeCriterion\_Tresca |
| Brittle materials | * swsFOSNonCompositeCriterion\_MohrCoulomb      - or   * swsFOSNonCompositeCriterion\_Coulomb |
| Pure beam studies | * swsFOSNonCompositeCriterion\_Automatic |

How you set stress limits using NStressLimitOption and NCompressiveStressLimitOption depends on the [model material](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWMaterial~ModelType.html).

| Specify NStressLimitOption and NCompressiveStressLimitOption with swsFactorOfSafetyStressLimitOption\_e... | For [swsMaterialModelType\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMaterialModelType_e.html)... |
| --- | --- |
| swsFactorOfSafetyStressLimitOption\_YieldStrength | * swsMaterialModelTypeLinearElasticIsotropic* swsMaterialModelTypeLinearElasticOrthtropic* swsMaterialModelTypeElastoPlasticvonMisesKinematic* swsMaterialModelTypeElastoPlasticTrescaKinematic |
| swsFactorOfSafetyStressLimitOption\_UltimateStrength | * swsMaterialModelTypeLinearElasticIsotropic* swsMaterialModelTypeLinearElasticOrthtropic* swsMaterialModelTypeNonlinearElastic* swsMaterialModelTypeElastoPlasticvonMmisesKinematic* swsMaterialModelTypeElastoPlasticTrescaKinematic* swsMaterialModelTypeElastoPlasticDruckerPrager* swsMaterialModelTypeHyperElasticBlatzko* swsMaterialModelTypeHyperElasticMooneyRivlin* swsMaterialModelTypeHyperElasticOgden* swsMaterialModelTypeViscoElastic* swsMaterialModelTypeNitinol |

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetMinMaxFactorOfSafety2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxFactorOfSafety2.html)

[ICWResults::GetFactorOfSafetyForComposites Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetFactorOfSafetyForComposites.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2018 SP0