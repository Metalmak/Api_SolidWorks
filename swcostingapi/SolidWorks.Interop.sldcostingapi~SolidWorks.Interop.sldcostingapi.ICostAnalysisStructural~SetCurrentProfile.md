<!-- source: swcostingapi/SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural~SetCurrentProfile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Costing API Help | Send Feedback |
| SetCurrentProfile Method (ICostAnalysisStructural) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldcostingapi Namespace](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi_namespace.html) > [ICostAnalysisStructural Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural.html) : SetCurrentProfile Method (ICostAnalysisStructural) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Standard*
:   Name of the profile standard (see **Remarks**)

*ProfileType*
:   Name of the profile type (see **Remarks**)

*ProfileSize*
:   Profile size (see **Remarks**)

Sets the profile for the weldment in this Costing analysis for this structural Costing analysis.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetCurrentProfile( _    ByVal Standard As System.String, _    ByVal ProfileType As System.String, _    ByVal ProfileSize As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICostAnalysisStructural Dim Standard As System.String Dim ProfileType As System.String Dim ProfileSize As System.String Dim value As System.Boolean   value = instance.SetCurrentProfile(Standard, ProfileType, ProfileSize) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetCurrentProfile(     System.string Standard,    System.string ProfileType,    System.string ProfileSize ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetCurrentProfile(  &   System.String^ Standard, &   System.String^ ProfileType, &   System.String^ ProfileSize ) ``` | |

#### Parameters

*Standard*
:   Name of the profile standard (see **Remarks**)

*ProfileType*
:   Name of the profile type (see **Remarks**)

*ProfileSize*
:   Profile size (see **Remarks**)

#### Return Value

True if the profile is set, false if not (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CostAnalysisStructural::SetCurrentProfile.

# ![](dotnetimages/collapse.gif)Remarks

|  |  |
| --- | --- |
| **A valid string for...** | **Corresponds to name of the...** |
| Standard | Weldment profile folder, typically located in **C:\Program Files\SolidWorks Corp\SOLIDWORKS**\**lang**\*lang*\**weldment profiles** |
| ProfileType | Profile types folder, typically located in **C:\Program Files\SolidWorks Corp\SOLIDWORKS**\**lang**\*lang*\**weldment profiles\***profile standard* |
| ProfileSize | Profile size file, excluding the filename extension, typically located in **C:\Program Files\SolidWorks Corp\SOLIDWORKS**\**lang**\*lang*\**weldment profiles\***profile standard**\**profile type* |

This method:

* does not change the underlying geometry of the structural member; instead, this method only uses the specified profile to cost the body.* fails if the specified Standard, ProfileType, or ProfileSize values are invalid or incompatible with each other.* could invalidate the [cost method](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural~CurrentCostMethodType.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICostAnalysisStructural Interface](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural.html)

[ICostAnalysisStructural Members](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural_members.html)

[ICostAnalysisStructural::CurrentProfileSize Property ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural~CurrentProfileSize.html)

[ICostAnalysisStructural::CurrentProfileStandard Property ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural~CurrentProfileStandard.html)

[ICostAnalysisStructural::CurrentProfileType Property ()](SolidWorks.Interop.sldcostingapi~SolidWorks.Interop.sldcostingapi.ICostAnalysisStructural~CurrentProfileType.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Costing API 2015 SP0