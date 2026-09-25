<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis_methods.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| IThicknessAnalysis Interface Methods | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) : IThicknessAnalysis Interface |

For a list of all members of this type, see [IThicknessAnalysis members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis_members.html).

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [Close](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~Close.html) | Ends the current session of a thickness analysis. |
| ![ Method](dotnetimages/Method.gif) | [GetAnalysisDetails](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetAnalysisDetails.html) | Gets the percentage of area and number of faces in each thickness range. |
| ![ Method](dotnetimages/Method.gif) | [GetAvgWeightedTckOnAnalArea](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetAvgWeightedTckOnAnalArea.html) | Gets the average weighted thickness on the analyzed area. |
| ![ Method](dotnetimages/Method.gif) | [GetAvgWeightedTckOnCritArea](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetAvgWeightedTckOnCritArea.html) | Gets the average weighted thickness on the critical area. |
| ![ Method](dotnetimages/Method.gif) | [GetCriticalFeatureNames](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetCriticalFeatureNames.html) | Gets the names of the features that violate the target thickness. |
| ![ Method](dotnetimages/Method.gif) | [GetCriticalSurfaceArea](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetCriticalSurfaceArea.html) | Gets the critical surface area. |
| ![ Method](dotnetimages/Method.gif) | [GetIntervalCount](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetIntervalCount.html) | Gets the number of intervals in the thickness color scale. |
| ![ Method](dotnetimages/Method.gif) | [GetMaxDeviationfromTargetThickness](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetMaxDeviationfromTargetThickness.html) | Gets the maximum deviation from the target thickness. |
| ![ Method](dotnetimages/Method.gif) | [GetMaxTckOnAnalArea](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetMaxTckOnAnalArea.html) | Gets the maximum thickness of the analyzed area. |
| ![ Method](dotnetimages/Method.gif) | [GetMinTckOnAnalArea](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetMinTckOnAnalArea.html) | Gets the minimum thickness of the analyzed area. |
| ![ Method](dotnetimages/Method.gif) | [GetNumCriticalFaces](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetNumCriticalFaces.html) | Gets the number of critical faces in the analyzed area. |
| ![ Method](dotnetimages/Method.gif) | [GetNumCriticalFeatures](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetNumCriticalFeatures.html) | Gets the number of critical features in the analyzed area. |
| ![ Method](dotnetimages/Method.gif) | [GetThicknessAnalysisBody](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetThicknessAnalysisBody.html) | Gets the SOLIDWORKS body in a multibody part selected for the thickness analysis. |
| ![ Method](dotnetimages/Method.gif) | [GetTotalSurfaceAreaAnalyzed](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetTotalSurfaceAreaAnalyzed.html) | Gets the total surface area analyzed. |
| ![ Method](dotnetimages/Method.gif) | [Init](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~Init.html) | Initializes the Thickness Analysis utility with the active SOLIDWORKS document. |
| ![ Method](dotnetimages/Method.gif) | [RunThickAnalysis](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~RunThickAnalysis.html) | Obsolete. Superseded by [IThicknessAnalysis::RunThickAnalysis2](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.IThicknessAnalysis~RunThickAnalysis2.html). |
| ![ Method](dotnetimages/Method.gif) | [RunThickAnalysis2](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~RunThickAnalysis2.html) | Runs a thickness analysis, shows the thick regions, and generates a report. |
| ![ Method](dotnetimages/Method.gif) | [RunThinAnalysis](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~RunThinAnalysis.html) | Obsolete. Superseded by [IThicknessAnalysis::RunThinAnalysis2](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.IThicknessAnalysis~RunThinAnalysis2.html). |
| ![ Method](dotnetimages/Method.gif) | [RunThinAnalysis2](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~RunThinAnalysis2.html) | Runs a thickness analysis, shows the thin regions, and generates a report. |
| ![ Method](dotnetimages/Method.gif) | [SetThicknessAnalysisBody](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~SetThicknessAnalysisBody.html) | Sets the SOLIDWORKS body in a multibody part to use in the thickness analysis. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IThicknessAnalysis Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis.html)

[SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html)