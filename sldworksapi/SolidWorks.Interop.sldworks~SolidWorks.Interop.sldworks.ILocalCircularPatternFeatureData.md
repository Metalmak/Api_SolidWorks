<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalCircularPatternFeatureData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ILocalCircularPatternFeatureData Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalCircularPatternFeatureData_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ILocalCircularPatternFeatureData Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to a circular component pattern feature in an assembly.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface ILocalCircularPatternFeatureData ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ILocalCircularPatternFeatureData ``` | |

| C# |  |
| --- | --- |
| ``` public interface ILocalCircularPatternFeatureData ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class ILocalCircularPatternFeatureData ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See LocalCircularPatternFeatureData.

# ![](dotnetimages/collapse.gif)Example

'VBA

'-------------------------------------------------------
' Preconditions: Verify that the assembly exists.
'
' Postconditions:
' 1. Opens the assembly.
' 2. Selects an edge for the direction axis.
' 3. Selects a subassembly to pattern.
' 4. Creates **LocalCirPattern1**.
' 5. Examine the FeatureManager design tree and
' graphics area.
'
' NOTE: Because the assembly is used elsewhere, do not
' save changes.
'--------------------------------------------------------
Option Explicit
Dim swApp As SldWorks.SldWorks
Dim swModel As SldWorks.ModelDoc2
Dim swModelDocExt As SldWorks.ModelDocExtension
Dim swFeatureManager As SldWorks.FeatureManager
Dim swFeature As SldWorks.Feature
Dim swLocalCirPattFD As SldWorks.LocalCircularPatternFeatureData
Dim status As Boolean
Dim errors As Long
Dim warnings As Long
Dim fileName As String
Sub main()

> Set swApp = Application.SldWorks
> fileName = "C:\Users\Public\Documents\SOLIDWORKS\SOLIDWORKS 2019\samples\tutorial\api\distance linkage.sldasm"
> Set swModel = swApp.OpenDoc6(fileName, swDocumentTypes\_e.swDocASSEMBLY, swOpenDocOptions\_e.swOpenDocOptions\_Silent, "", errors, warnings)
> Set swModelDocExt = swModel.Extension
> Set swFeatureManager = swModel.FeatureManager
> status = swModelDocExt.SelectByID2("", "EDGE", 0.22639417933982, -0.194822643434378, 0.102086175644843, False, 2, Nothing, 0)
> status = swModelDocExt.SelectByID2("mount base-1@distance linkage", "COMPONENT", 0, 0, 0, True, 1, Nothing, 0)
> Set swLocalCirPattFD = swFeatureManager.**CreateDefinition**(swFmLocalCirPattern)
> swLocalCirPattFD.**TotalInstances** = 3
> swLocalCirPattFD.**EqualSpacing** = True
> Set swFeature = swFeatureManager.**CreateFeature**(swLocalCirPattFD)
> swModel.ClearSelection2 True

End Sub

# ![](dotnetimages/collapse.gif)Example

[Get and Set Seed Components (C#)](Get_and_Set_Seed_Components_Example_CSharp.htm)

[Get and Set Seed Components (VB.NET)](Get_and_Set_Seed_Components_Example_VBNET.htm)

[Get and Set Seed Components (VBA)](Get_and_Set_Seed_Components_Example_VB.htm)

[Create Local Circular Pattern (C#)](Create_Local_Circular_Pattern_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Read Pattern Features and their Feature Data Objects.

Before calling IFeatureManager::CreateDefinition, you can pre-select the entities needed to create the local circular pattern feature.

| If... | To select a component, use... |
| --- | --- |
| Using [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) to select components, ordered selection of the components is required | * 1 to mark the components to pattern * 2 to mark the axis |
| Directly selecting a component or axis | [ISelectData::Mark](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectData~Mark.html) and [Component2::Select3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IComponent2~Select3.html)   * 1 to mark the components to pattern * 2 to mark the axis |

Or, after calling IFeatureManger::CreateDefinition, you can explicitly set the corresponding properties on the feature data object.

Either way, you must call [IFeatureManager::CreateFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateFeature.html) after initializing this feature data object in order to successfully create the local circular pattern feature.

# ![](dotnetimages/collapse.gif)Accessors

[IFeature::GetDefinition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetDefinition.html)

[IFeatureManager::CreateDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateDefinition.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[LocalCircularPatternFeatureData](SWObjectModel.pdf#LocalCircularPatternFeatureData)

# ![](dotnetimages/collapse.gif)See Also

####

[ILocalCircularPatternFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ILocalCircularPatternFeatureData_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)

[ICircularPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICircularPatternFeatureData.html)