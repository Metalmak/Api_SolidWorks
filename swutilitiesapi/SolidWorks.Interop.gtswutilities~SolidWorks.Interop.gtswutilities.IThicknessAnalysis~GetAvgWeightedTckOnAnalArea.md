<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetAvgWeightedTckOnAnalArea.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| GetAvgWeightedTckOnAnalArea Method (IThicknessAnalysis) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [IThicknessAnalysis Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis.html) : GetAvgWeightedTckOnAnalArea Method (IThicknessAnalysis) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*lErrorcode*
:   Error as defined in [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

Gets the average weighted thickness on the analyzed area.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetAvgWeightedTckOnAnalArea( _    ByRef lErrorcode As System.Integer _ ) As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IThicknessAnalysis Dim lErrorcode As System.Integer Dim value As System.Double   value = instance.GetAvgWeightedTckOnAnalArea(lErrorcode) ``` | |

| C# |  |
| --- | --- |
| ``` System.double GetAvgWeightedTckOnAnalArea(     out System.int lErrorcode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.double GetAvgWeightedTckOnAnalArea(  &   [Out] System.int lErrorcode ) ``` | |

#### Parameters

*lErrorcode*
:   Error as defined in [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

#### Return Value

Average weighted thickness on analyzed area

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See IThicknessAnalysis::GetAvgWeightedTckOnAnalArea.

# ![](dotnetimages/collapse.gif)Example

[Run Thickness Analysis (VBA)](Run_Thickness_Analysis_VB6.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IThicknessAnalysis Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis.html)

[IThicknessAnalysis Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis_members.html)

[IThicknessAnalysis::GetAvgWeightedTckOnAnalArea Method](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetAvgWeightedTckOnAnalArea.html)

[IThicknessAnalysis::GetMaxTckOnAnalArea Method](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetMaxTckOnAnalArea.html)

[IThicknessAnalysis::GetMinTckOnAnalArea Method](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetMinTckOnAnalArea.html)

[IThicknessAnalysis::GetTotalSurfaceAreaAnalyzed Method](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetTotalSurfaceAreaAnalyzed.html)

[IThicknessAnalysis::GetAvgWeightedTckOnCritArea Method](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IThicknessAnalysis~GetAvgWeightedTckOnCritArea.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2006 FCS