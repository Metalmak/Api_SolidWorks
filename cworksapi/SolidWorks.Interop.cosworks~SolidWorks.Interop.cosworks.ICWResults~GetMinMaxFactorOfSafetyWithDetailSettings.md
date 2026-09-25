<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxFactorOfSafetyWithDetailSettings.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetMinMaxFactorOfSafetyWithDetailSettings Method (ICWResults) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetMinMaxFactorOfSafetyWithDetailSettings Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BAllBodies*
:   True to select all bodies to plot the factor of safety, false to select specific bodies

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
:   Tensile stress limit as defined in [swsFactorOfSafetyStressLimitOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFactorOfSafetyStressLimitOption_e.html)

*DStressValue*
:   Tensile stress value; valid only if NStressLimitOption is swsFactorOfSafetyStressLimitOption\_e.swsFactorOfSafetyStressLimitOption\_UserDefined

*NCompressiveStressLimitOption*
:   Compressive stress limit as defined in swsFactorOfSafetyStressLimitOption\_e

*DCompressiveStressValue*
:   Compressive stress value; valid only if NCompressiveStressLimitOption is swsFactorOfSafetyStressLimitOption\_e.swsFactorOfSafetyStressLimitOption\_UserDefined

*DMultiplicationFactor*
:   Tensile stress limit multiplication factor

*DCompressiveStressMultiplicationFactor*
:   Compressive stress limit multiplication factor

*BCombinedStressOnBeams*
:   True to combine stress on beams, false to not

*NShellOptions*
:   Shell face on which to perform the factor of safety as defined by [swsFOS\_ShellFaceOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFOS_ShellFaceOption_e.html)

*ErrorCode*
:   Error code as defined by [swsFosPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFosPlotErrorCode_e.html)

Obsolete. Superseded by [ICWResults::GetMinMaxFactorOfSafetyWithDetailSettings2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxFactorOfSafetyWithDetailSettings2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetMinMaxFactorOfSafetyWithDetailSettings( _    ByVal BAllBodies As System.Boolean, _    ByVal ArraySelectedEntities As System.Object, _    ByVal NComponent As System.Integer, _    ByVal BUpperLimit As System.Boolean, _    ByVal DUpperValue As System.Double, _    ByVal NStressUnit As System.Integer, _    ByVal NStressLimitOption As System.Integer, _    ByVal DStressValue As System.Double, _    ByVal NCompressiveStressLimitOption As System.Integer, _    ByVal DCompressiveStressValue As System.Double, _    ByVal DMultiplicationFactor As System.Double, _    ByVal DCompressiveStressMultiplicationFactor As System.Double, _    ByVal BCombinedStressOnBeams As System.Boolean, _    ByVal NShellOptions As System.Integer, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim BAllBodies As System.Boolean Dim ArraySelectedEntities As System.Object Dim NComponent As System.Integer Dim BUpperLimit As System.Boolean Dim DUpperValue As System.Double Dim NStressUnit As System.Integer Dim NStressLimitOption As System.Integer Dim DStressValue As System.Double Dim NCompressiveStressLimitOption As System.Integer Dim DCompressiveStressValue As System.Double Dim DMultiplicationFactor As System.Double Dim DCompressiveStressMultiplicationFactor As System.Double Dim BCombinedStressOnBeams As System.Boolean Dim NShellOptions As System.Integer Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetMinMaxFactorOfSafetyWithDetailSettings(BAllBodies, ArraySelectedEntities, NComponent, BUpperLimit, DUpperValue, NStressUnit, NStressLimitOption, DStressValue, NCompressiveStressLimitOption, DCompressiveStressValue, DMultiplicationFactor, DCompressiveStressMultiplicationFactor, BCombinedStressOnBeams, NShellOptions, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetMinMaxFactorOfSafetyWithDetailSettings(     System.bool BAllBodies,    System.object ArraySelectedEntities,    System.int NComponent,    System.bool BUpperLimit,    System.double DUpperValue,    System.int NStressUnit,    System.int NStressLimitOption,    System.double DStressValue,    System.int NCompressiveStressLimitOption,    System.double DCompressiveStressValue,    System.double DMultiplicationFactor,    System.double DCompressiveStressMultiplicationFactor,    System.bool BCombinedStressOnBeams,    System.int NShellOptions,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetMinMaxFactorOfSafetyWithDetailSettings(  &   System.bool BAllBodies, &   System.Object^ ArraySelectedEntities, &   System.int NComponent, &   System.bool BUpperLimit, &   System.double DUpperValue, &   System.int NStressUnit, &   System.int NStressLimitOption, &   System.double DStressValue, &   System.int NCompressiveStressLimitOption, &   System.double DCompressiveStressValue, &   System.double DMultiplicationFactor, &   System.double DCompressiveStressMultiplicationFactor, &   System.bool BCombinedStressOnBeams, &   System.int NShellOptions, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*BAllBodies*
:   True to select all bodies to plot the factor of safety, false to select specific bodies

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
:   Tensile stress limit as defined in [swsFactorOfSafetyStressLimitOption\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFactorOfSafetyStressLimitOption_e.html)

*DStressValue*
:   Tensile stress value; valid only if NStressLimitOption is swsFactorOfSafetyStressLimitOption\_e.swsFactorOfSafetyStressLimitOption\_UserDefined

*NCompressiveStressLimitOption*
:   Compressive stress limit as defined in swsFactorOfSafetyStressLimitOption\_e

*DCompressiveStressValue*
:   Compressive stress value; valid only if NCompressiveStressLimitOption is swsFactorOfSafetyStressLimitOption\_e.swsFactorOfSafetyStressLimitOption\_UserDefined

*DMultiplicationFactor*
:   Tensile stress limit multiplication factor

*DCompressiveStressMultiplicationFactor*
:   Compressive stress limit multiplication factor

*BCombinedStressOnBeams*
:   True to combine stress on beams, false to not

*NShellOptions*
:   Shell face on which to perform the factor of safety as defined by [swsFOS\_ShellFaceOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFOS_ShellFaceOption_e.html)

*ErrorCode*
:   Error code as defined by [swsFosPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFosPlotErrorCode_e.html)

#### Return Value

Array of two doubles of the minimum and maximum factors of safety

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetMinMaxFactorOfSafetyWithDetailSettings.

# ![](dotnetimages/collapse.gif)Remarks

For pure beam studies, you can only specify NComponent with swsFOS\_NonCompositeCriterion\_e.swsFOSNonCompositeCriterion\_Automatic.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetMinMaxFactorOfSafety Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxFactorOfSafety.html)

[ICWResults::GetFactorOfSafetyForComposites Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetFactorOfSafetyForComposites.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2015 SP0