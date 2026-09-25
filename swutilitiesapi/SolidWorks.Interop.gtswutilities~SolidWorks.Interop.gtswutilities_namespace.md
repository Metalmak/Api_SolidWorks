<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| SolidWorks.Interop.gtswutilities Namespace | |
| [See Also](#seealsobookmark)  [Inheritance Hierarchy](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace_hierarchy.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

SOLIDWORKS Utilities API

# ![](dotnetimages/collapse.gif)Interfaces

| Interface | Description |
| --- | --- |
| [ICompareDocument](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareDocument.html) | Compares the properties of two SOLIDWORKS documents. |
| [ICompareFeature](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareFeature.html) | Identifies the differences in solid features between two versions of the same part. |
| [ICompareGeometry](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareGeometry.html) | Identifies the differences in geometry in both solid features and surface models between two versions of the same part. |
| [IFeaturePaint](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IFeaturePaint.html) | Allows you to copy the feature parameters from one feature in a SOLIDWORKS part to a feature in a different SOLIDWORKS part. |
| [IFindReplaceAnnotations](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IFindReplaceAnnotations.html) | Finds and replaces text for the annotations in the currently open part, assembly, or drawing document. |
| [IGeometryAnalysis](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IGeometryAnalysis.html) | Identifies geometric entities in a part that could cause a problem in other applications. |
| [IPowerSelect](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IPowerSelect.html) | Allows selection of entities (edges, loops, faces, or features) in a part that meet the specified criteria. |
| [IThicknessAnalysis](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis.html) | Allows you to determine and analyze the thickness of a part. |
| [IUtilities](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IUtilities.html) | Gets the SOLIDWORKS Utilities tool interface and options. |
| [IUtilOptions](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IUtilOptions.html) | Gets or sets the angular and position tolerance options when comparing faces. |

# ![](dotnetimages/collapse.gif)Enumerations

| Enumeration | Description |
| --- | --- |
| [gtCodOperationOption\_e](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.gtCodOperationOption_e.html) | Options for comparing documents. Bitmask. |
| [gtError\_e](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.gtError_e.html) | Error codes returned by SOLIDWORKS Utilities APIs. |
| [gtFraFilterType\_e](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.gtFraFilterType_e.html) | Types of annotations. Bitmask. |
| [gtFraOptionType\_e](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.gtFraOptionType_e.html) | Options to use to filter a search for a find and replace annotation operation. Bitmask. |
| [gtGdfOperationOption\_e](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.gtGdfOperationOption_e.html) | Comparison options. |
| [gtpslEdgeAngleOperator\_e](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.gtpslEdgeAngleOperator_e.html) | Edge-angle operator types for [IPowerSelect](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.IPowerSelect.html). |
| [gtpslFeatureType\_e](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.gtpslFeatureType_e.html) | Feature type IDs for [IPowerSelect](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.IPowerSelect.html). |
| [gtpslFilterType\_e](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.gtpslFilterType_e.html) | Filter types for [IPowerSelect](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.IPowerSelect.html). Bitmask. |
| [gtPslSelectionType\_e](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.gtPslSelectionType_e.html) | Select types for [IPowerSelect](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.IPowerSelect.html). Bitmask. |
| [gtResultOptions\_e](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.gtResultOptions_e.html) | Options for results reporting. |
| [gtSwTools\_e](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.gtSwTools_e.html) | Tool IDs for [IUtilities::GetToolInterface](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.IUtilities~GetToolInterface.html). |
| [gttckResolutionOptions\_e](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.gttckResolutionOptions_e.html) | Resolution options for [IThicknessAnalysis](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.IThicknessAnalysis.html). |
| [gtVolDiffStatusOptionType\_e](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.gtVolDiffStatusOptionType_e.html) | Error types returned by [ICompareGeometry::CompareGeometry3](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.ICompareGeometry~CompareGeometry3.html). |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.gtswutilities Assembly](SolidWorks.Interop.gtswutilities.html)