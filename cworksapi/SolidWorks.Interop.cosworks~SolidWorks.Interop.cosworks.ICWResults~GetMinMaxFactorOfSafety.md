<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxFactorOfSafety.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetMinMaxFactorOfSafety Method (ICWResults) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetMinMaxFactorOfSafety Method (ICWResults) |

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

*NShellOptions*
:   Shell face on which to perform the factor of safety as defined by [swsFOS\_ShellFaceOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFOS_ShellFaceOption_e.html)

*ErrorCode*
:   Error code as defined by [swsFosPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFosPlotErrorCode_e.html)

Obsolete. Superseded by [ICWResults::GetMinMaxFactorOfSafety2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxFactorOfSafety2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetMinMaxFactorOfSafety( _    ByVal BAllBodies As System.Boolean, _    ByVal ArraySelectedEntities As System.Object, _    ByVal NComponent As System.Integer, _    ByVal NShellOptions As System.Integer, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim BAllBodies As System.Boolean Dim ArraySelectedEntities As System.Object Dim NComponent As System.Integer Dim NShellOptions As System.Integer Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetMinMaxFactorOfSafety(BAllBodies, ArraySelectedEntities, NComponent, NShellOptions, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetMinMaxFactorOfSafety(     System.bool BAllBodies,    System.object ArraySelectedEntities,    System.int NComponent,    System.int NShellOptions,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetMinMaxFactorOfSafety(  &   System.bool BAllBodies, &   System.Object^ ArraySelectedEntities, &   System.int NComponent, &   System.int NShellOptions, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*BAllBodies*
:   True to select all bodies to plot the factor of safety, false to select specific bodies

*ArraySelectedEntities*
:   Array of bodies for which to plot the factor of safety; valid only if BAllBodies is set to false

*NComponent*
:   Failure criterion as defined by [swsFOS\_NonCompositeCriterion\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsFOS_NonCompositeCriterion_e.html) (see **Remarks**)

*NShellOptions*
:   Shell face on which to perform the factor of safety as defined by [swsFOS\_ShellFaceOption\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFOS_ShellFaceOption_e.html)

*ErrorCode*
:   Error code as defined by [swsFosPlotErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsFosPlotErrorCode_e.html)

#### Return Value

Array of two doubles of the minimum and maximum factors of safety

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetMinMaxFactorOfSafety.

# ![](dotnetimages/collapse.gif)Remarks

For pure beam studies, you can only specify NComponent with swsFOS\_NonCompositeCriterion\_e.swsFOSNonCompositeCriterion\_Automatic.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

[ICWResults::GetFactorOfSafetyForComposites Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetFactorOfSafetyForComposites.html)

[ICWResults::GetMinMaxFactorOfSafetyWithDetailSettings Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetMinMaxFactorOfSafetyWithDetailSettings.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2013 SP5.0