<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsUserPreferenceIntegerValue_e.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| swsUserPreferenceIntegerValue\_e Enumeration | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All  Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : swsUserPreferenceIntegerValue\_e Enumeration |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

User preference integer values

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Enum swsUserPreferenceIntegerValue_e     Inherits System.Enum ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As swsUserPreferenceIntegerValue_e ``` | |

| C# |  |
| --- | --- |
| ``` public enum swsUserPreferenceIntegerValue_e : System.Enum ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public enum class swsUserPreferenceIntegerValue_e : public System.Enum ``` | |

# ![](dotnetimages/collapse.gif)Members

| Member | Description |
| --- | --- |
| **swsColorChartColorOptionBaseChartColorNumber** | 23 = Get or set the number of colors in the color chart; corresponds to **Simulation > Options > Default Options > Plot > Color Chart > Color Options > No of chart colors** |
| **swsColorChartColorOptionChartColorNumber** | 22 = Get or set the user-defined number of colors in the color chart; corresponds to **Simulation > Options > Default Options > Plot > Color Chart > Color Options > User defined** |
| **swsColorChartColorOptionLegendType** | 24 = Get or set the color legend type as defined in [swsColorChartOptionLegendTypeValue\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsColorChartOptionLegendTypeValue_e.html); corresponds to **Simulation > Options > Default Options > Plot > Color Chart > Color Options > (Default, Rainbow, Gray scale, User Defined)** |
| **swsColorChartColorOptionvonMisesColorValue** | 27 = Get or set the color for values above yield for vonMises plots; corresponds to **Simulation > Options > Default Options > Plot > Color Chart > Color Options > Specify color for values above yield for vonMises plot** |
| **swsColorChartNumberFormatLegendPrecision** | 25 = Get or set the number of decimal places for precision of number formats; corresponds to **Simulation > Options > Default Options > Plot > Color Chart > Number format > No. of decimal places:** |
| **swsColorChartNumberFormatOption** | 21 = Get or set the number format as defined in [swsColorChartNumberFormatOptionValue\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsColorChartNumberFormatOptionValue_e.html); corresponds to **Simulation > Options > Default Options > Plot > Color Chart > Number format > (Scientific, Floating, or General)** |
| **swsColorChartNumberFormatUseDiffNoFormatOption** | 26 = Get or set which notation other than scientific to use for small numbers as defined in [swsColorNumberFormatUseDiffNumberFormatOptionValue\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsColorNumberFormatUseDiffNumberFormatOptionValue_e.html); corresponds to **Simulation > Options > Default Options > Plot > Color Chart > Number format > Scientific > Use different number format for small numbers (0.001 < |x| < 1000) > (Floating or General)** |
| **swsColorChartPosition** | 3 = Get or set the position of the color bar as defined in [swsColorChartPositionValue\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsColorChartPositionValue_e.html); corresponds to **Simulation > Options > Default Options > Plot > Color Chart > Position > (Predefined positions or user defined)** |
| **swsColorChartPositionUserDefinedXValue** | 18 = Get or set the color bar's horizontal distance from the left of the graphics area as a percentage of the width of the window; corresponds to **Simulation > Options > Default Options > Plot > Color Chart > Position > User defined > Horizontal from left:** |
| **swsColorChartPositionUserDefinedYValue** | 19 = Get or set the color bar's vertical distance from the top of the graphics area as a percentage of the height of the window; corresponds to **Simulation > Options > Default Options > Plot > Color Chart > Position > User defined > Vertical from top:** |
| **swsColorChartWidthOption** | 20 = Get or set the color chart width as defined in [swsColorChartWidthOptionValue\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsColorChartWidthOptionValue_e.html); corresponds to **Simulation > Options > Default Options > Plot > Color Chart > Width** |
| **swsDefaultResultFolder** | 1 = Get or set the results folder option as defined in [swsResultFolderValue\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsResultFolderValue_e.html); corresponds to **Simulation > Options > Default Options > Results > Results folder > (SOLIDWORKS document folder or User defined)** |
| **swsDefaultSolverValue** | 0 = Get or set the default solver as defined in [swsSolverType\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsSolverType_e.html); corresponds to **Simulation > Options > Default Options > Results > Default Solver > (Automatic, Direct sparse, or FFEPlus)** |
| **swsEMailType** | 30 |
| **swsMesherType** | 31 = Get or set the mesher type as defined in [swsMesherTypeNew\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsMesherTypeNew_e.html) |
| **swsPlotBoundaryOptionMeshColor** | 9 = Get or set the mesh color for boundaries (see **Remarks**); corresponds to **Simulation > Options > Default Options > Plot > Settings options > Boundary options > Mesh > color select box** |
| **swsPlotBoundaryOptionModelColor** | 29 = Get or set the model color for boundaries (see **Remarks**); corresponds to **Simulation > Options > Default Options > Plot > Settings options > Boundary options > Model** |
| **swsPlotBoundaryOptionTranslucentSingleColorSetting** | 8 = Get or set the translucent color for boundaries (see **Remarks**); corresponds to **Simulation > Options > Default Options > Plot > Settings options > Boundary options > Translucent (Single color) > color select box** |
| **swsPlotDeformedShapeOptionSetSuperImposeOption** | 16 = Get or set the translucent color option for superimposing the model on deformed shape as defined in [swsPlotDeformedShapeOptionSuperImposeValue\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsPlotDeformedShapeOptionSuperImposeValue_e.html); corresponds to **Simulation > Options > Default Options > Plot > Deformed shape options > Show results on deformed shape > Superimpose model on deformed shape > Translucent (part colors or single color)** |
| **swsPlotDeformedShapeOptionSetting** | 12 = Get or set how to show deformed shape results as defined in [swsPlotDeformedShapeOptionValue\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsPlotDeformedShapeOptionValue_e.html); corresponds to **Simulation > Options > Default Options > Plot > Deformed shape options > Show results on undeformed shape or Show results on deformed shape** |
| **swsPlotDeformedShapeOptionTranslucentColor** | 28 = Get or set the translucent color for superimposing the model on deformed shape (see **Remarks**);  corresponds to **Simulation > Options > Default Options > Plot > Deformed shape options > Show results on deformed shape > Superimpose model on deformed shape > Translucent (single color) > color select box** |
| **swsPlotDeformedShapeResultOther** | 15 = Get or set the deformation scale factor for all other studies as defined in [swsPlotDeformedShapeOptionScaleFactorOtherValue\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsPlotDeformedShapeOptionScaleFactorOtherValue_e.html); corresponds to **Simulation > Options > Default Options > Plot > Deformed shape options > Show results on deformed shape > Deformation scale factor for: > all other studies: > Automatic or True(1.0)** |
| **swsPlotDeformedShapeResultScaleContact** | 13 = Get or set the deformation scale factor for all studies with "No penetration" contact as defined in [swsPlotDeformedShapeOptionScaleFactorContactValue\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsPlotDeformedShapeOptionScaleFactorContactValue_e.html); corresponds to **Simulation > Options > Default Options > Plot > Deformed shape options > Show results on deformed shape > Deformation scale factor for: > all studies with "No penetration" contact: > Automatic or True(1.0)** |
| **swsPlotDeformedShapeResultScaleLarge** | 14 = Get or set the deformation scale factor for studies with the "Large displacement" option as defined in [swsPlotDeformedShapeOptionScaleFactorLargeDispValue\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsPlotDeformedShapeOptionScaleFactorLargeDispValue_e.html); corresponds to **Simulation > Options > Default Options > Plot > Deformed shape options > Show results on deformed shape > Deformation scale factor for: > studies with the "Large displacement" option: > Automatic or True(1.0)** |
| **swsPlotSettingsBoundaryOption** | 5 = Get or set the boundary option as defined in [swsPlotBoundarySettingsOptionValue\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsPlotBoundarySettingsOptionValue_e.html); corresponds to **Simulation > Options > Default Options > Plot > Settings options > Boundary options** |
| **swsPlotSettingsFringeOption** | 4 = Get or set the fringe option as defined in [swsPlotFringeSettingsOptionValue\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsPlotFringeSettingsOptionValue_e.html); corresponds to **Simulation > Options > Default Options > Plot > Settings options > Fringe options** |
| **swsPlotShowExcludedBodiesOption** | 6 = Get or set the translucent color option for excluded bodies as defined in [swsPlotShowExcludedBodiesOptionValue\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsPlotShowExcludedBodiesOptionValue_e.html); corresponds to **Simulation > Options > Default Options > Plot > Settings options > Show excluded bodies > Translucent (Single color or Part colors)** |
| **swsPlotShowExcludedBodyTranslucentSingleColor** | 10 = Get or set the translucent color for all excluded bodies (see **Remarks**);  corresponds to **Simulation > Options > Default Options > Plot > Settings options > Show excluded bodies > Translucent (Single color) > color select box** |
| **swsPlotShowHiddenBodiesOption** | 7 = Get or set the translucent color option for hidden bodies as defined in [swsPlotShowHiddenBodiesOptionValue\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsPlotShowHiddenBodiesOptionValue_e.html); corresponds to **Simulation > Options > Default Options > Plot > Settings options > Show hidden bodies > Translucent (Single color or Part colors)** |
| **swsPlotShowHiddenBodyTranslucentSingleColor** | 11 = Get or set the translucent color for all hidden bodies (see **Remarks**); corresponds to **Simulation > Options > Default Options > Plot > Settings options > Show hidden bodies > Translucent (Single color) > color select box** |
| **swsReportPublishOption** | 2 = Get or set the report folder location as defined in [swsReportFolderValue\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsReportFolderValue_e.html); corresponds to **Simulation > Options > Default Options > Report > Report publish options > Report folder** |
| **swsReportPublishOptionReportFolderUserDefinedPath** | 17 |

# ![](dotnetimages/collapse.gif)See Also

####

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)