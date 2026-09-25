<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ITablePatternFeatureData Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ITablePatternFeatureData Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to a table-driven pattern feature.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface ITablePatternFeatureData ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITablePatternFeatureData ``` | |

| C# |  |
| --- | --- |
| ``` public interface ITablePatternFeatureData ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class ITablePatternFeatureData ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See TablePatternFeatureData.

# ![](dotnetimages/collapse.gif)Example

'VBA

' \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
' 1. Open *public\_documents***\samples\tutorial\api\tablepattern.sldprt**.
' 2. Delete **TPattern1**.
' 3. Run the macro.
' 4. Creates a new **TPattern1**.
' 5. Inspect the FeatureManager design tree and the graphics area.
' \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Dim swApp As SldWorks.SldWorks
Dim swFeatData As TablePatternFeatureData
Dim Part As SldWorks.ModelDoc2
Dim swFeat As Feature
Dim swFeatMgr As FeatureManager
Dim boolstatus As Boolean

Option Explicit
Sub main()

> Set swApp = Application.SldWorks
> Set Part = swApp.ActiveDoc
>
> boolstatus = Part.Extension.SelectByID2("Coordinate System1", "COORDSYS", 0, 0, 0, True, 16, Nothing, 0)
> boolstatus = Part.Extension.SelectByID2("Cut-Extrude1", "BODYFEATURE", 0, 0, 0, True, 4, Nothing, 0)
> Part.ActivateSelectedFeature
> Dim swPointArray() As Double
> ReDim swPointArray(0 To 5) As Double
> swPointArray(0) = 0.04
> swPointArray(1) = 0
> swPointArray(2) = 0
> swPointArray(3) = -0.025
> swPointArray(4) = 0
> swPointArray(5) = 0
>
> Set swFeatMgr = Part.FeatureManager
>
> Set swFeatData = swFeatMgr.**CreateDefinition**(swFmTablePattern)
> swFeatData.**GeometryPattern** = False
> swFeatData.**PointArray** = swPointArray
> swFeatData.**PropagateVisualProperty** = True
> swFeatData.**UseCentroid** = True
> Set swFeat = swFeatMgr.**CreateFeature**(swFeatData)

End Sub

# ![](dotnetimages/collapse.gif)Example

[Get Points of Repeating Elements in Table-driven Pattern (C#)](Get_Points_of_Repeating_Elements_in_Table-driven_Pattern_Example_CSharp.htm)

[Get Points of Repeating Elements in Table-driven Pattern (VB.NET)](Get_Points_of_Repeating_Elements_in_Table-driven_Pattern_Example_VBNET.htm)

[Get Points of Repeating Elements in Table-driven Pattern (VBA)](Get_Points_of_Repeating_Elements_in_Table-driven_Pattern_Example_VB.htm)

[Create Table Pattern (C#)](Create_Table_Pattern_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Read Pattern Features and their Feature Data Objects.

Before calling IFeatureManager::CreateDefinition, you can pre-select the entities needed to create the table-driven pattern feature.

| **To** [**select**](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html)**...** | Use mark... |
| --- | --- |
| Seed feature | 4 |
| Coordinate system | 16 |
| Reference point | 32 |
| Seed face | 128 |
| Seed body | 256 |

Or, after calling IFeatureManager::CreateDefinition, you can explicitly set the corresponding properties on this feature data object.

Either way, you must call [IFeatureManager::CreateFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateFeature.html) after initializing this feature data object in order to successfully create the table-driven pattern.

See the **Table Driven Patterns** topic in the SOLIDWORKS user-interface help for more information about table-driven patterns.

# ![](dotnetimages/collapse.gif)Accessors

[IFeature::GetDefinition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetDefinition.html)

[IFeatureManager::CreateDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateDefinition.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[TablePatternFeatureData](SWObjectModel.pdf#TablePatternFeatureData)

# ![](dotnetimages/collapse.gif)See Also

####

[ITablePatternFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITablePatternFeatureData_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)