<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~AddSMNormalCutType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddSMNormalCutType Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : AddSMNormalCutType Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*AutoPropagation*
:   True to automatically propagate the Normal Cut, false to not

*Optimize*
:   True to optimize geometry, false to not

*BExtent*
:   True to maximize the cutout using the top and bottom intersection profiles, false to use an offset plane

Obsolete. See [IFeatureManager::CreateFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateFeature.html) and the Remarks in [ISMNormalCutGroupData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutGroupData.html), and [ISMNormalCutFeatureData2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub AddSMNormalCutType( _    ByVal AutoPropagation As System.Boolean, _    ByVal Optimize As System.Boolean, _    ByVal BExtent As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim AutoPropagation As System.Boolean Dim Optimize As System.Boolean Dim BExtent As System.Boolean   instance.AddSMNormalCutType(AutoPropagation, Optimize, BExtent) ``` | |

| C# |  |
| --- | --- |
| ``` void AddSMNormalCutType(     System.bool AutoPropagation,    System.bool Optimize,    System.bool BExtent ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void AddSMNormalCutType(  &   System.bool AutoPropagation, &   System.bool Optimize, &   System.bool BExtent ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*AutoPropagation*
:   True to automatically propagate the Normal Cut, false to not

*Optimize*
:   True to optimize geometry, false to not

*BExtent*
:   True to maximize the cutout using the top and bottom intersection profiles, false to use an offset plane

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::AddSMNormalCutType.

# ![](dotnetimages/collapse.gif)Example

```
'VBA
```

```
'1. Open a sheet metal part that has two cut extrudes.
'2. Modify the macro below as needed.
```

```
Dim swApp As SldWorks.SldWorks
Dim Part As SldWorks.ModelDoc2
Dim myFeature As SldWorks.Feature
Dim myNormalCutFeatData As SldWorks.SMNormalCutFeatureData
Dim boolstatus As Boolean
```

```
Option Explicit
Sub main()
```

```
    Set swApp = Application.SldWorks
    Set Part = swApp.ActiveDoc
```

```
    'Select a cut-extrude face for which to create a Normal Cut
    boolstatus = Part.Extension.SelectByRay(-6.38655841527864E-02, -1.56055561574817E-02, 3.58410081097382E-03, -9.80322952634684E-02, -0.994744620924993, -2.95433279467378E-02, 2.7317052985792E-04, 2, False, 1, 0)
    Dim OneFaceGroup As Long
    OneFaceGroup = Part.FeatureManager.AddSMNormalCut()
    Part.ClearSelection2 True

    'Use an offset plane to create the Normal Cut feature
    boolstatus = Part.Extension.SelectByRay(-6.00249578326526E-02, -1.83129588701831E-02, 1.70249820822459E-02, -9.80322952634684E-02, -0.994744620924993, -2.95433279467378E-02, 2.69645748827495E-04, 2, False, 4, 0)
```

```
    Part.FeatureManager.AddSMNormalCutType True, True, False

    'Create a Normal Cut feature using the previously selected cut-extrude faces
    Set myFeature = Part.FeatureManager.FinishSMNormalCut()
```

```
    Set swFeatData = myFeature.GetDefinition
    Dim Number As Long
    Number = swFeatData.GetNumberOfFaceGroups()
```

```
    'Select another cut-extrude face for which to create a second Normal Cut
    boolstatus = swFeatData.AccessSelections(Part, Nothing)

    boolstatus = Part.Extension.SelectByRay(-6.24756020285346E-02, -1.97848124440725E-02, 1.18685503457829E-02, -9.80322952634684E-02, -0.994744620924993, -2.95433279467378E-02, 2.7317052985792E-04, 2, False, 1, 0)
    Dim instance As ISelectionMgr
    Set face = Part.SelectionManager.GetSelectedObject6(1, -1)
    Dim faces As Variant
    Dim aFaces() As SldWorks.face
    ReDim aFaces(0)
    Set aFaces(0) = face
    faces = aFaces
    longwarnings = swFeatData.AddAGroupOfFaces(faces, longwarnings)

    Number = swFeatData.GetNumberOfFaceGroups()
```

```
    'Change the profile of the Normal Cut by adjusting the offset of the offset plane
    myNormalCutFeatData.Offset = 1.0

    Dim bStatus As Boolean
    bStatus = myFeature.ModifyDefinition(swFeatData, Part, Nothing)
    Part.ClearSelection2 True

End Sub
```

# ![](dotnetimages/collapse.gif)Remarks

To create a Normal Cut feature in a sheet metal part, call:

1. [IFeatureManager::AddSMNormalCut](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~AddSMNormalCut.html).- IFeatureManager::AddSMNormalCutType.- [IModelDocExtension::SelectByID2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByID2.html) with Mark = 1 to select the cut-extrude faces that you wish to make Normal Cuts.- IModelDocExtension::SelectByID2 with Mark = 2 to select the group of cut-extrude faces.- IModelDocExtension::SelectByID2 with Mark = 4 to select the offset plane, if BExtent is false.- (Optional) IModelDocExtension::SelectByID2 with Mark = 8 to select the direction of normal cut, if BExtent is true.- [IFeatureManager::FinishSMNormalCut](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FinishSMNormalCut.html).- [ISMNormalCutFeatureData::Offset](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData~Offset.html) to change the profile of the Normal Cut.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[ISMNormalCutFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISMNormalCutFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0