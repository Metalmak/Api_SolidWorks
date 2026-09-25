<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertGlobalBoundingBox.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertGlobalBoundingBox Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertGlobalBoundingBox Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BBoxType*
:   Bounding Box fit type as defined in swGlobalBoundingBoxFitOptions\_e (see **Remarks**)

*IncludeHiddenBodies*
:   True to include hidden bodies, false to not

*IncludeSurfaceBodies*
:   True to include surfaces, false to not

*Status*
:   Status as defined by swGlobalBoundingBoxResult\_e

Obsolete. See [IFeatureManager::CreateDefinition](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~CreateDefinition.html) and [IBoundingBoxFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBoundingBoxFeatureData.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertGlobalBoundingBox( _    ByVal BBoxType As System.Integer, _    ByVal IncludeHiddenBodies As System.Boolean, _    ByVal IncludeSurfaceBodies As System.Boolean, _    ByRef Status As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim BBoxType As System.Integer Dim IncludeHiddenBodies As System.Boolean Dim IncludeSurfaceBodies As System.Boolean Dim Status As System.Integer Dim value As System.Object   value = instance.InsertGlobalBoundingBox(BBoxType, IncludeHiddenBodies, IncludeSurfaceBodies, Status) ``` | |

| C# |  |
| --- | --- |
| ``` System.object InsertGlobalBoundingBox(     System.int BBoxType,    System.bool IncludeHiddenBodies,    System.bool IncludeSurfaceBodies,    out System.int Status ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ InsertGlobalBoundingBox(  &   System.int BBoxType, &   System.bool IncludeHiddenBodies, &   System.bool IncludeSurfaceBodies, &   [Out] System.int Status ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BBoxType*
:   Bounding Box fit type as defined in swGlobalBoundingBoxFitOptions\_e (see **Remarks**)

*IncludeHiddenBodies*
:   True to include hidden bodies, false to not

*IncludeSurfaceBodies*
:   True to include surfaces, false to not

*Status*
:   Status as defined by swGlobalBoundingBoxResult\_e

#### Return Value

[IFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertGlobalBoundingBox.

# ![](dotnetimages/collapse.gif)Example

```
'VBA
```

```
Dim swApp As SldWorks.SldWorks
Dim Part As SldWorks.ModelDoc2
Dim boolstatus As Boolean
Dim longstatus As Long
Option Explicit
```

```
Sub main()

    Set swApp = Application.SldWorks
    Set Part = swApp.ActiveDoc
```

```
    ' Display the Bounding Box sketch
    boolstatus = Part.SetUserPreferenceToggle)swViewDispGlobalBBox, True)

    Dim BoundingBox As SldWorks.Feature
    Set BoundingBox = Part.FeatureManager.InsertGlobalBoundingBox(swBoundingBoxType_BestFit, True, False, longstatus)
```

```
    Part.ClearSelection2 True
```

```
    ' Hide the Bounding Box sketch
    boolstatus = Part.SetUserPreferenceToggle)swViewDispGlobalBBox, False)
```

```
End Sub
```

# ![](dotnetimages/collapse.gif)Remarks

If BBoxType is set to swGlobalBoundingBoxFitOptions\_e.swBoundingBoxType\_CustomPlane, then select a face or plane using [IModelDocExtension::SelectByRay](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByRay.html) with TypeWanted set to swSelectType\_e.swSelFACES before calling this method.

To display or hide the Bounding Box sketch, call [IModelDoc2::SetUserPreferenceToggle](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~SetUserPreferenceToggle.html) to set swUserPreferenceToggle\_e.swViewDispGlobalBBox to true or false, respectively.

After calling this method, use [IModelDoc2::ClearSelection2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~ClearSelection2.html) to clear the selection made when the Bounding Box is created.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0