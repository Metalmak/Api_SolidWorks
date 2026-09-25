<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISlotMateFeatureData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISlotMateFeatureData Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISlotMateFeatureData_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ISlotMateFeatureData Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to a slot mate feature.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface ISlotMateFeatureData ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISlotMateFeatureData ``` | |

| C# |  |
| --- | --- |
| ``` public interface ISlotMateFeatureData ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class ISlotMateFeatureData ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SlotMateFeatureData.

# ![](dotnetimages/collapse.gif)Example

'VBA
' \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
' 1. Open *public\_documents***\samples\tutorial\api\MechanicalMates\slot\_slot.sldasm**.
' 2. Run the macro.
' 3. Inspect the Mates folder of the FeatureManager design tree.
' \*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*
Dim swApp As SldWorks.SldWorks
Dim Part As SldWorks.ModelDoc2
Dim boolstatus As Boolean
Option Explicit

Sub main()

> Set swApp = Application.SldWorks
>
> Set Part = swApp.ActiveDoc
> boolstatus = Part.Extension.SelectByRay(0.12649032355856, 0.133857958976421, 8.79467058769023E-03, 3.53905007657348E-02, 0.579257713320296, 0.814375843216443, 2.14371287556113E-03, 2, True, 1, 0)
> boolstatus = Part.Extension.SelectByRay(9.59257342875013E-02, 9.99222046038994E-02, -2.51429018803719E-02, 3.53905007657348E-02, 0.579257713320296, 0.814375843216443, 2.14371287556113E-03, 2, True, 1, 0)
>
> ' Create SlotMateFeatureData
> Dim MateData As SldWorks.SlotMateFeatureData
> Set MateData = Part.**CreateMateData**(21)
>
> ' Set the entities to mate
> Dim EntitiesToMate(1) As Object
> Set EntitiesToMate(0) = Part.SelectionManager.GetSelectedObject6(1, -1)
> Set EntitiesToMate(1) = Part.SelectionManager.GetSelectedObject6(2, -1)
> Dim EntitiesToMateVar As Variant
> EntitiesToMateVar = EntitiesToMate
> MateData.**EntitiesToMate** = (EntitiesToMateVar)
>
> ' Set the mate alignment
> MateData.**MateAlignment** = 0
>
> ' Set the mate constraint
> MateData.**Constraint** = 0
>
> ' Create the mate
> Dim MateFeature As SldWorks.Feature
> Set MateFeature = Part.**CreateMate**(MateData)
> Part.ClearSelection2 True
> Part.EditRebuild3

End Sub

# ![](dotnetimages/collapse.gif)Example

[Create Slot Mate (C#)](Create_Slot_Mate_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

A slot mate is a mate between:

* A bolt and either a straight slot or an arced slot.* Two slots, straight or arced

[IMateFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMateFeatureData.html) is the parent of this mate interface.

To create a slot mate:

1. Follow general instructions in the [IAssemblyDoc::CreateMate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~CreateMate.html) Remarks.- Specify [ISlotMateFeatureData::EntitiesToMate](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISlotMateFeatureData~EntitiesToMate.html) or use [IModelDocExtension::SelectByID2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByID2.html) to pre-select the entities using Mark = 1.- Specify other properties of the SlotMateFeatureData object. as required.

To edit a slot mate:

1. Access its feature and call [IFeature::GetDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~GetDefinition.html) to get the MateFeatureData object.- Cast the MateFeatureData object to a SlotMateFeatureData object.- Modify the SlotMateFeatureData object.- Call [IFeature::ModifyDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~ModifyDefinition.html).

To delete this slot mate, use [IModelDocExtension::DeleteSelection2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~DeleteSelection2.html).

# ![](dotnetimages/collapse.gif)Access Diagram

[SlotMateFeatureData](SWObjectModel.pdf#SlotMateFeatureData)

# ![](dotnetimages/collapse.gif)See Also

####

[ISlotMateFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISlotMateFeatureData_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)