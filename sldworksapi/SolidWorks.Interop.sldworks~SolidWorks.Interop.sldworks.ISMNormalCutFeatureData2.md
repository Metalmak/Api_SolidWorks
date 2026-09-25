<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ISMNormalCutFeatureData2 Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData2_members.html)   [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : ISMNormalCutFeatureData2 Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to a sheet metal normal cut feature.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface ISMNormalCutFeatureData2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISMNormalCutFeatureData2 ``` | |

| C# |  |
| --- | --- |
| ``` public interface ISMNormalCutFeatureData2 ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class ISMNormalCutFeatureData2 ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SMNormalCutFeatureData2.

# ![](dotnetimages/collapse.gif)Example

'VBA

'\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*

'1. Open **c:\Users\Public\Documents\SOLIDWORKS\SOLIDWORKS 2019\samples\whatsnew\sheet metal\normal\_cut.sldprt**.
'2. Open the Immediate window.
'3. Run the macro.
'4. Creates **Normal Cut1** in the FeatureManager design tree.
'5. Edits the feature by specifying a normal cut direction entity.
'6. Inspect the Immediate window.

'\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*\*

Option Explicit
Dim swApp As SldWorks.SldWorks
Dim swModel As SldWorks.ModelDoc2
Dim swModelDocExt As SldWorks.ModelDocExtension
Dim swFeatMgr As SldWorks.FeatureManager
Dim swFeat As SldWorks.Feature
Dim swNormalCutFeatData As SldWorks.SMNormalCutFeatureData2
Dim grpData As SldWorks.SMNormalCutGroupData
Dim swSelMgr As SldWorks.SelectionMgr
Dim swCutDirectionFace As SldWorks.Face2
Dim errCode As Long
Dim boolstatus As Boolean
Dim varGrpNames As Variant
Dim i As Long
Dim j As Long
Dim Name As String
Dim Face As SldWorks.Face2

Sub main()

    Set swApp = Application.SldWorks
    Set swModel = swApp.**ActiveDoc**
    Set swModelDocExt = swModel.**Extension**
    Set swFeatMgr = swModel.**FeatureManager**
    Set swNormalCutFeatData = swFeatMgr.**CreateDefinition**(swFmNormalCut)
    swNormalCutFeatData.**AutoPropagation** = True
    swNormalCutFeatData.**OptimizeGeometry** = True
    swNormalCutFeatData.**NormalCutParameters** = swNormalCutExtent

    ' Select the face(s) to make normal

    boolstatus = swModel.**Extension**.**SelectByRay**(4.71296104838217E-02, 1.42054003862171E-02, -6.68923799798904E-03, -0.13322686545804, 0.182153484913837, 0.974202602261958, 6.19874904830013E-04, 2, True, 1, 0)

    Set grpData = swNormalCutFeatData.**CreateGroup**(errCode)

    ' Create the normal cut feature

    Set swFeat = swFeatMgr.**CreateFeature**(swNormalCutFeatData)

    ' Modify the normal cut feature

    Set swNormalCutFeatData = swFeat.**GetDefinition**()
    swNormalCutFeatData.**AccessSelections** swModel, Nothing
    varGrpNames = swNormalCutFeatData.**GetGroupNames**()

    For i = 0 To UBound(varGrpNames)
        Name = varGrpNames(i)
        Debug.Print "GroupName: " & Name
        Set grpData = swNormalCutFeatData.**GetGroupByName**(Name)
        Dim varFaces As Variant
        varFaces = grpData.**Faces**
        For j = 0 To UBound(varFaces)
            Set Face = varFaces(j)
            Debug.Print "Face " & j & " area: " & Face.**GetArea**
        Next j
        Debug.Print "--------------------"
    Next i

    'Specify the cut direction

    Set swSelMgr = swModel.**SelectionManager**
    boolstatus = swModel.**Extension**.**SelectByRay**(-0.149999999999892, 2.58556514245498E-02, -4.63505465353364E-03, 0.393242668518252, 0.12460738379391, -0.910951811876282, 1.22626958447854E-03, 2, False, 0, 0)
    Set swCutDirectionFace = Nothing
    Set swCutDirectionFace = swSelMgr.**GetSelectedObject6**(1, -1)

    Dim swSelectEnt As SldWorks.Entity
    Set swSelectEnt = swCutDirectionFace
    boolstatus = swSelectEnt.**Select4**(False, Nothing)
    swNormalCutFeatData.**CutDirection** = swCutDirectionFace

    Dim isModified As Boolean
    isModified = swFeat.**ModifyDefinition**(swNormalCutFeatData, swModel, Nothing)

End Sub

# ![](dotnetimages/collapse.gif)Example

[Create Normal Cut Feature (C#)](Create_Normal_Cut_Feature_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Extruded cuts that pierce models at an angle have non-normal side walls. To make these side walls normal, you create a normal cut feature.

To create a normal cut feature:

1. Open a sheet metal part that has a cut-extrude with non-normal side walls.- Call IFeatureManager::CreateDefinition(swFmNormalCut) to access this interface.- Set non-entity properties on this interface.- Use [IModelDocExtension::SelectByRay](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByRay.html) or [IModelDocExtension::SelectByID2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByID2.html) with Mark = 4 to select the offset plane, only if [ISMNormalCutFeatureData2::NormalCutParameters](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData2~NormalCutParameters.html) is set to swNormalCutParameters\_e.swNormalCutOffsetPlane.- Use IModelDocExtension::SelectByRay or IModelDocExtension::SelectByID2 with Mark = 8 to select the direction of the normal cut, only if ISMNormalCutFeatureData2::NormalCutParameters is set to swNormalCutParameters\_e.swNormalCutExtent.- Use IModelDocExtension::SelectByRay or IModelDocExtension::SelectByID2 with Mark = 1 to select each non-normal face in the group. If [ISMNormalCutFeatureData2::AutoPropagation](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData2~AutoPropagation.html) is set to true, then all faces tangent to a selected face are automatically added to the face group.- Call [ISMNormalCutFeatureData2::CreateGroup](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData2~CreateGroup.html) to access [ISMNormalCutGroupData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutGroupData.html).- Repeat steps 6 and 7 as many times as you have face groups. Call [IModelDoc2::ClearSelection2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ClearSelection2.html) after each face group is created.- Call [IFeatureManager::CreateFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateFeature.html).

To edit a normal cut feature:

1. Call IFeature::GetDefinition to get this feature data object for a selected normal cut feature.- Call [ISMNormalCutFeatureData2::AccessSelections](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData2~AccessSelections.html). **Note:** **Any selections made \**before\** this call are invalid. To edit the properties of this feature, you must re-select their entities during the editing session, i.e., after calling ISMNormalCutFeatureData2::AccessSelections. (See step 5.)**- Call [ISMNormalCutFeatureData2::GetGroupNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData2~GetGroupNames.html) and [ISMNormalCutFeatureData2::GetGroupByName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData2~GetGroupByName.html) to access ISMNormalCutGroupData for an existing face group.- Call ISMNormalCutFeatureData2::CreateGroup to create another face group if needed.- Modify [cut direction](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData2~CutDirection.html), [offset plane reference](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData2~OffsetPlaneReference.html), or other properties on ISMNormalCutFeatureData2 as needed. To select property entities, use IModelDocExtension::SelectByRay or IModelDocExtension::SelectByID2 followed by [ISelectionMgr::GetSelectedObject6](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectionMgr~GetSelectedObject6.html). You can also use [IEntity::Select4](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEntity~Select4.html).- Call [IFeature::ModifyDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature~ModifyDefinition.html) if you modifed the feature or [ISMNormalCutFeatureData2::ReleaseSelectionAccess](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData2~ReleaseSelectionAccess.html) if you did not.

# ![](dotnetimages/collapse.gif)Accessors

[IFeature::GetDefinition](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature~GetDefinition.html)

[IFeatureManager::CreateDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateDefinition.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[SMNormalCutFeatureData2](SWObjectModel.pdf#SMNormalCutFeatureData2)

# ![](dotnetimages/collapse.gif)See Also

####

[ISMNormalCutFeatureData2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData2_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)