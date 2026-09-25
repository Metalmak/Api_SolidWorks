<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxFactorOfSafety2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetMinMaxFactorOfSafety2 Method (ICWResults) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetMinMaxFactorOfSafety2 Method (ICWResults) |

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

*NShellOptions*
:   Shell face on which to perform the factor of safety as defined by [swsFOS\_ShellFaceOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFOS_ShellFaceOption_e.html)

*NStepNumber*
:   Plot step number or 0; 0 gets step 1 for linear static studies and the last available plot step for nonlinear static studies

*ErrorCode*
:   Error code as defined by [swsFosPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFosPlotErrorCode_e.html)

Gets the algebraic minimum and maximum factors of safety (FOS) for non-composite shells.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetMinMaxFactorOfSafety2( _    ByVal BAllBodies As System.Boolean, _    ByVal ArraySelectedEntities As System.Object, _    ByVal NComponent As System.Integer, _    ByVal NShellOptions As System.Integer, _    ByVal NStepNumber As System.Integer, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim BAllBodies As System.Boolean Dim ArraySelectedEntities As System.Object Dim NComponent As System.Integer Dim NShellOptions As System.Integer Dim NStepNumber As System.Integer Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetMinMaxFactorOfSafety2(BAllBodies, ArraySelectedEntities, NComponent, NShellOptions, NStepNumber, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetMinMaxFactorOfSafety2(     System.bool BAllBodies,    System.object ArraySelectedEntities,    System.int NComponent,    System.int NShellOptions,    System.int NStepNumber,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetMinMaxFactorOfSafety2(  &   System.bool BAllBodies, &   System.Object^ ArraySelectedEntities, &   System.int NComponent, &   System.int NShellOptions, &   System.int NStepNumber, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*BAllBodies*
:   True to use all bodies to plot the factor of safety, false to use specific bodies

*ArraySelectedEntities*
:   Array of bodies for which to plot the factor of safety; valid only if BAllBodies is set to false

*NComponent*
:   Failure criterion as defined by [swsFOS\_NonCompositeCriterion\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFOS_NonCompositeCriterion_e.html) (see **Remarks**)

*NShellOptions*
:   Shell face on which to perform the factor of safety as defined by [swsFOS\_ShellFaceOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFOS_ShellFaceOption_e.html)

*NStepNumber*
:   Plot step number or 0; 0 gets step 1 for linear static studies and the last available plot step for nonlinear static studies

*ErrorCode*
:   Error code as defined by [swsFosPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFosPlotErrorCode_e.html)

#### Return Value

Array of two doubles of the minimum and maximum factors of safety

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetMinMaxFactorOfSafety2.

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

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetMinMaxFactorOfSafetyWithDetailSettings2 Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxFactorOfSafetyWithDetailSettings2.html)

[ICWResults::GetFactorOfSafetyForComposites Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetFactorOfSafetyForComposites.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2018 SP0