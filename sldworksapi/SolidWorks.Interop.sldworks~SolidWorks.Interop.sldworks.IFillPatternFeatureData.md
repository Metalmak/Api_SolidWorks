<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFillPatternFeatureData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IFillPatternFeatureData Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFillPatternFeatureData_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IFillPatternFeatureData Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to a fill pattern feature.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IFillPatternFeatureData ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFillPatternFeatureData ``` | |

| C# |  |
| --- | --- |
| ``` public interface IFillPatternFeatureData ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IFillPatternFeatureData ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FillPatternFeatureData.

# ![](dotnetimages/collapse.gif)Example

'VBA

'\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
'1. Ensure the specified part exists.
'2. Run the macro.
'3. Inspect the graphics area and the FeatureManager design tree.
'\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*

Dim swApp As SldWorks.SldWorks
Dim myFeature As SldWorks.Feature
Dim swFeat As SldWorks.Feature
Dim swFeatMgr As SldWorks.FeatureManager
Dim Part As SldWorks.ModelDoc2
Dim swFeatData As SldWorks.FillPatternFeatureData
Dim boolstatus As Boolean
Dim longstatus As Long, longwarnings As Long
Option Explicit
Sub main()

> Set swApp = Application.SldWorks
>
> Set Part = swApp.OpenDoc6("C:\Users\Public\Documents\SOLIDWORKS\SOLIDWORKS 2019\samples\tutorial\api\block20.sldprt", 1, 0, "", longstatus, longwarnings)
> swApp.ActivateDoc2 "block20.sldprt", False, longstatus
> Set Part = swApp.ActiveDoc

> boolstatus = Part.Extension.SelectByRay(-0.044420257315096, 3.96239999998329E-02, -3.92581286577638E-02, -0.400036026779312, -0.515038074910024, -0.758094294050284, 1.1224765174324E-03, 2, False, 0, 0)
>
> Set myFeature = Part.FeatureManager.SimpleHole2(0.0054, True, False, False, 1, 0, 0.0254, 0.0254, False, False, False, False, 1.74532925199433E-02, 1.74532925199433E-02, False, False, False, False, True, True, True, True, False)
> Part.SelectionManager.EnableContourSelection = False
> Part.ActivateSelectedFeature
>
> boolstatus = Part.Extension.SelectByID2("Hole1", "BODYFEATURE", 0, 0, 0, False, 4, Nothing, 0)
> boolstatus = Part.Extension.SelectByRay(1.06119575008097E-03, 0.039624, 4.93456023787655E-02, -0.400036026779312, -0.515038074910024, -0.758094294050284, 1.1224765174324E-03, 1, True, 1, 0)
> boolstatus = Part.Extension.SelectByRay(6.36836165047043E-02, 3.96239999998329E-02, -6.33171793538168E-04, -0.400036026779312, -0.515038074910024, -0.758094294050284, 1.1224765174324E-03, 2, True, 16384, 0)
>
> Set swFeatMgr = Part.FeatureManager
>
> Set swFeatData = swFeatMgr.**CreateDefinition**(swFmFillPattern)
> swFeatData.**CreateSeedCutPolygonSides** = 0
> swFeatData.**CreateSeedCutType** = 0
> swFeatData.**Diagonal** = 0.008
> swFeatData.**Diameter** = 0.008
> swFeatData.**Dimension** = 5.65685424949238E-03
> swFeatData.**FeaturesToPatternType** = 0
> swFeatData.**GeometryPattern** = False
> swFeatData.**InnerRadius** = 3.80422606518061E-03
> swFeatData.**InstanceSpacing** = 1.70240490494193E-02
> swFeatData.**LayoutSpacingType** = 1
> swFeatData.**LoopSpacing** = 1.70240490494193E-02
> swFeatData.**Margins** = 0
> swFeatData.**NoOfInstances** = 10
> swFeatData.**OuterRadius** = 0.004
> swFeatData.**PatternLayoutPolygonSides** = 0
> swFeatData.**PatternLayoutType** = 0
> swFeatData.**Rotation** = 0
> swFeatData.**SeedCutFlipShapeDirection** = False
> swFeatData.**StaggerAngle** = 1.0471975511966
> Set swFeat = swFeatMgr.**CreateFeature**(swFeatData)

End Sub

# ![](dotnetimages/collapse.gif)Example

[Create Fill Pattern (C#)](Create_Fill_Pattern_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Read Pattern Features and their Feature Data Objects.

Before calling IFeatureManager::CreateDefinition, you can pre-select the entities needed to create the fill pattern feature.

> | Use [IModelDocExtension::SelectByID2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByID2.html) to select... | For the Fill Pattern's... | Using Mark... |
> | --- | --- | --- |
> | Sketch, face, planar curve on a face, or coplanar faces | Fill boundary | 16384 |
> | Direction reference (e.g., edge or axis) | Pattern direction (if not selected, SOLIDWORKS chooses a direction reference appropriate for the specified layout) | 1 |
> | Vertex or sketch point | Location of the pattern seed instance (if a point is not selected, the pattern seed instance is placed at the center of the fill boundary region) | 3 |
> | Features | Pattern objects | 4 |
> | Faces | Pattern objects | 5 |
> | Bodies | Pattern objects | 6 |

Or, after calling IFeatureManager::CreateDefinition, you can explicitly set the corresponding properties on the feature data object. You can also initialize:

> * [IFillPatternFeatureData::PatternLayoutType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFillPatternFeatureData~PatternLayoutType.html)* [IFillPatternFeatureData::LayoutSpacingType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFillPatternFeatureData~LayoutSpacingType.html)* [IFillPatternFeatureData::FeaturesToPatternType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFillPatternFeatureData~FeaturesToPatternType.html)* [IFillPatternFeatureData::GeometryPattern](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFillPatternFeatureData~GeometryPattern.html)* [IFillPatternFeatureData::LoopSpacing](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFillPatternFeatureData~LoopSpacing.html) (for all PatternLayoutTypes except swPatternLayoutType\_e.swPatternLayoutPerforation)* Depending on the settings above, other properties might need to be initialized.

Either way, you must call [IFeatureManager::CreateFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateFeature.html) after initializing this feature data object in order to successfully create the fill pattern feature.

For all pattern layouts except swPatternLayoutType\_e.swPatternLayoutPerforation, the fill pattern is created by positioning a pattern seed instance within the fill boundary and copying the pattern in concentric loops about the seed instance.

See the **Fill Pattern PropertyManager** topic in the SOLIDWORKS Help for more information about fill pattern features.

# ![](dotnetimages/collapse.gif)Accessors

[IFeature::GetDefinition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetDefinition.html)

[IFeatureManager::CreateDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateDefinition.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[FillPatternFeatureData](SWObjectModel.pdf#FillPatternFeatureData)

# ![](dotnetimages/collapse.gif)See Also

####

[IFillPatternFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFillPatternFeatureData_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)