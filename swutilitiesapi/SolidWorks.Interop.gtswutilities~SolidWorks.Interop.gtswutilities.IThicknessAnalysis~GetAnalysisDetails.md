<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetAnalysisDetails.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| GetAnalysisDetails Method (IThicknessAnalysis) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [IThicknessAnalysis Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis.html) : GetAnalysisDetails Method (IThicknessAnalysis) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*lRange*
:   1-based index of the number of intervals in the thickness color scale (see **Remarks**)

*dMinTckInRange*
:   Minimum thickness of thickness range

*dMaxTckInRange*
:   Maximum thickness of thickness range

*lNoFaces*
:   Number of faces

*dSurfArea*
:   Surface area

*dPerAnalArea*
:   Percent of total area analyzed that falls in the specified thickness range

Gets the percentage of area and number of faces in each thickness range.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetAnalysisDetails( _    ByVal lRange As System.Integer, _    ByRef dMinTckInRange As System.Double, _    ByRef dMaxTckInRange As System.Double, _    ByRef lNoFaces As System.Integer, _    ByRef dSurfArea As System.Double, _    ByRef dPerAnalArea As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IThicknessAnalysis Dim lRange As System.Integer Dim dMinTckInRange As System.Double Dim dMaxTckInRange As System.Double Dim lNoFaces As System.Integer Dim dSurfArea As System.Double Dim dPerAnalArea As System.Double Dim value As System.Integer   value = instance.GetAnalysisDetails(lRange, dMinTckInRange, dMaxTckInRange, lNoFaces, dSurfArea, dPerAnalArea) ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetAnalysisDetails(     System.int lRange,    out System.double dMinTckInRange,    out System.double dMaxTckInRange,    out System.int lNoFaces,    out System.double dSurfArea,    out System.double dPerAnalArea ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetAnalysisDetails(  &   System.int lRange, &   [Out] System.double dMinTckInRange, &   [Out] System.double dMaxTckInRange, &   [Out] System.int lNoFaces, &   [Out] System.double dSurfArea, &   [Out] System.double dPerAnalArea ) ``` | |

#### Parameters

*lRange*
:   1-based index of the number of intervals in the thickness color scale (see **Remarks**)

*dMinTckInRange*
:   Minimum thickness of thickness range

*dMaxTckInRange*
:   Maximum thickness of thickness range

*lNoFaces*
:   Number of faces

*dSurfArea*
:   Surface area

*dPerAnalArea*
:   Percent of total area analyzed that falls in the specified thickness range

#### Return Value

Error as defined in [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See IThicknessAnalysis::GetAnalysisDetails.

# ![](dotnetimages/collapse.gif)Example

[Run Thickness Analysis (VBA)](Run_Thickness_Analysis_VB6.htm)

# ![](dotnetimages/collapse.gif)Remarks

Use [IThicknessAnalysis::GetIntervalCount](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.IThicknessAnalysis~GetIntervalCount.html) to get the number of intervals in the thickness color scale.

# ![](dotnetimages/collapse.gif)See Also

####

[IThicknessAnalysis Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis.html)

[IThicknessAnalysis Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis_members.html)

[IThicknessAnalysis::GetAvgWeightedTckOnCritArea Method](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetAvgWeightedTckOnCritArea.html)

[IThicknessAnalysis::GetCriticalFeatureNames Method](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetCriticalFeatureNames.html)

[IThicknessAnalysis::GetCriticalSurfaceArea Method](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetCriticalSurfaceArea.html)

[IThicknessAnalysis::GetMaxDeviationfromTargetThickness Method](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetMaxDeviationfromTargetThickness.html)

[IThicknessAnalysis::GetNumCriticalFaces Method](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetNumCriticalFaces.html)

[IThicknessAnalysis::GetNumCriticalFeatures Method](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetNumCriticalFeatures.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2006 FCS