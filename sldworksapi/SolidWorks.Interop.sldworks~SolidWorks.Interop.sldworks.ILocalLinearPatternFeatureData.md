<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ILocalLinearPatternFeatureData Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ILocalLinearPatternFeatureData Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to a linear component pattern feature in an assembly.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface ILocalLinearPatternFeatureData ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ILocalLinearPatternFeatureData ``` | |

| C# |  |
| --- | --- |
| ``` public interface ILocalLinearPatternFeatureData ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class ILocalLinearPatternFeatureData ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See LocalLinearPatternFeatureData.

# ![](dotnetimages/collapse.gif)Example

'VBA

'--------------------------------------------------
' Preconditions: Verify that the assembly exists.
'
' Postconditions:
' 1. Opens the assembly.
' 2. Selects an edge for Direction 1.
' 3. Selects a subassembly to pattern.
' 4. Creates a local linear pattern.
' 5. Examine the FeatureManager design tree and
' graphics area.
'
' NOTE: Because the assembly is used elsewhere, do
' not save changes.
'---------------------------------------------------
Option Explicit
Dim swApp As SldWorks.SldWorks
Dim swModel As SldWorks.ModelDoc2
Dim swModelDocExt As SldWorks.ModelDocExtension
Dim swFeatureManager As SldWorks.FeatureManager
Dim swFeature As SldWorks.Feature
Dim swLocalLinearPatternFD As SldWorks.LocalLinearPatternFeatureData
Dim status As Boolean
Dim errors As Long
Dim warnings As Long
Dim fileName As String
Sub main()

> Set swApp = Application.SldWorks
> fileName = "C:\Users\Public\Documents\SOLIDWORKS\SOLIDWORKS 2020\samples\tutorial\api\distance linkage.sldasm"
>
> Set swModel = swApp.OpenDoc6(fileName, swDocumentTypes\_e.swDocASSEMBLY, swOpenDocOptions\_e.swOpenDocOptions\_Silent, "", errors, warnings)
>
> Set swModelDocExt = swModel.Extension
>
> Set swFeatureManager = swModel.FeatureManager
>
> status = swModelDocExt.SelectByID2("", "EDGE", 0.222723097227572, -0.193386735236572, -0.10172211746567, False, 2, Nothing, 0)
>
> status = swModelDocExt.SelectByID2("mount base-1 @ distance linkage", "COMPONENT", 0, 0, 0, True, 1, Nothing, 0)
>
> Set swLocalLinearPatternFD = swFeatureManager.**CreateDefinition**(swFmLocalLPattern)
>
> swLocalLinearPatternFD.**D1ReverseDirection** = True
> swLocalLinearPatternFD.**D1Spacing** = 0.1516
> swLocalLinearPatternFD.**D1TotalInstances** = 4
> swLocalLinearPatternFD.**D2PatternSeedOnly** = False
> swLocalLinearPatternFD.**D2ReverseDirection** = False
> swLocalLinearPatternFD.**D2Spacing** = 0.05
> swLocalLinearPatternFD.**D2TotalInstances** = 1
> swLocalLinearPatternFD.**SynchronizeFlexibleComponents** = False
>
> Set swFeature = swFeatureManager.**CreateFeature**(swLocalLinearPatternFD)
>
> swModel.ClearSelection2 True
> swModel.ViewZoomtofit2

End Sub

# ![](dotnetimages/collapse.gif)Example

[Get and Set Seed Components (C#)](Get_and_Set_Seed_Components_Example_CSharp.htm)

[Get and Set Seed Components (VB.NET)](Get_and_Set_Seed_Components_Example_VBNET.htm)

[Get and Set Seed Components (VBA)](Get_and_Set_Seed_Components_Example_VB.htm)

[Create Local Linear Pattern (C#)](Create_Local_Linear_Pattern_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Read Pattern Features and their Feature Data Objects.

Before calling [IFeatureManager::CreateDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateDefinition.html), you must pre-select the D1 and D2 end (and seed) reference entities to create the linear component pattern feature.

| If... | To select an up-to entity (vertex, edge, face, or plane), use... | To select a body, use... | To select a component, use... |
| --- | --- | --- | --- |
| Using [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) to select entities, solid bodies, or components requires ordered selection | * Mark = 256 to select the Direction 1 end reference* Mark = 512 to select the Direction 1 end seed reference* Mark = 1024 to select the Direction 2 end reference* Mark = 2048 to select the Direction 2 end seed reference | * Mark = 1 to mark Direction 1* Mark = 256 to mark the solid bodies to pattern | * Mark = 1 to mark the components to pattern * Mark = 2 to mark Direction 1 and Mark = 4 to mark Direction 2 |
| Directly selecting an entity, solid body, or component | [IEntity::Select4](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEntity~Select4.html) with:   * [ISelectData::Mark](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectData~Mark.html) = 256 to select the Direction 1 end reference* ISelectData::Mark = 512 to select the Direction 1 end seed reference* ISelectData::Mark = 1024 to select the Direction 2 end reference* ISelectData::Mark = 2048 to select the Direction 2 end seed reference | * IEntity::Select4 with ISelectData::Mark = 1 to mark Direction 1  * [IBody2::Select2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~Select2.html) with ISelectData::Mark = 256 to mark the bodies to pattern | * [IComponent2::Select4](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IComponent2~Select4.html)  and ISelectData::Mark = 1 to mark the components to pattern  * IEntity::Select4 and ISelectData::Mark = 2 for Direction 1; Mark=4 for Direction 2 |

After calling IFeatureManager::CreateDefinition, you can further initialize the feature data object using:

* [ILocalLinearPatternFeatureData::D1Axis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData~D1Axis.html) to specify Direction 1.

* [ILocalLinearPatternFeatureData::SeedComponentArray](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData~SeedComponentArray.html) to specify the pattern's seed components.

* [ILocalLinearPatternFeatureData::D1EndCondition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData~D1EndCondition.html) to specify either spacing and instances or offsetting from an up-to reference:

**If explicitly setting pattern spacing and number of pattern instances, use:**

* [ILocalLinearPatternFeatureData::D1Spacing](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData~D1Spacing.html) to specify spacing between pattern instances.* [ILocalLinearPatternFeatureData::D1TotalInstances](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData~D1TotalInstances.html) to specify the number of pattern instances.* [ILocalLinearPatternFeatureData::D1ReverseDirection](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData~D1ReverseDirection.html) to reverse Direction 1.* [ILocalLinearPatternFeatureData::RotateInstances](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData~RotateInstances.html) to rotate pattern instances. If true:

* Use [ILocalLinearPatternFeatureData::RotationAngle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData~RotationAngle.html).* Use [ILocalLinearPatternFeatureData::RotationAxis](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData~RotationAxis.html).* Use [ILocalLinearPatternFeatureData::FixedAxisOfRotation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData~FixedAxisOfRotation.html). If true: Use [ILocalLinearPatternFeatureData::AlignToSeed](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData~AlignToSeed.html). If true:
      Use [ILocalLinearPatternFeatureData::SeedAlignmentReferencePoint](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData~SeedAlignmentReferencePoint.html).

**If offsetting from an up-to reference, use:**

* + [ILocalLinearPatternFeatureData::D1EndRefOffset](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData~D1EndRefOffset.html) to specify the distance between the last pattern instance and the up-to reference.

  + [ILocalLinearPatternFeatureData::D1EndRefReverseOffset](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData~D1EndRefReverseOffset.html) to reverse the offset.+ [ILocalLinearPatternFeatureData::D1EndUseSpacing](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData~D1EndUseSpacing.html) to specify either spacing or number of instances (one or the other, not both):
      - If true, use ILocalLinearPatternFeatureData::D1Spacing.- If false, use ILocalLinearPatternFeatureData::D1TotalInstances.* All of the ILocalLinearPatternFeatureData::D2\* properties to specify Direction 2 for a bidirectional linear component pattern.* Other properties such as [instances to skip](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILinearPatternFeatureData~SkippedItemArray.html) and [synchronize movement of flexible subassembly components](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData~SynchronizeFlexibleComponents.html).

You must call [IFeatureManager::CreateFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateFeature.html) after initializing this feature data object in order to successfully create the linear pattern feature.

For more information, see the **Linear Component Pattern PropertyManager** topic in the SOLIDWORKS user-interface help.

# ![](dotnetimages/collapse.gif)Accessors

[IFeature::GetDefinition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetDefinition.html)

IFeatureManager::CreateDefinition

# ![](dotnetimages/collapse.gif)Access Diagram

[LocalLinearPatternFeatureData](SWObjectModel.pdf#LocalLinearPatternFeatureData)

# ![](dotnetimages/collapse.gif)See Also

####

[ILocalLinearPatternFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalLinearPatternFeatureData_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[ILinearPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILinearPatternFeatureData.html)