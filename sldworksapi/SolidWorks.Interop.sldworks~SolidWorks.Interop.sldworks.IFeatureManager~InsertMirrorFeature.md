<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMirrorFeature.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertMirrorFeature Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertMirrorFeature Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BMirrorBody*
:   True to mirror solid bodies; false to mirror a feature or face

*BGeometryPattern*
:   True to mirror only the feature geometry, false to solve the entire feature; applies
    to mirroring features only

*BMerge*
:   True to merge any mirrored solid bodies, false to not; applies to mirroring solid
    bodies only

*BKnit*
:   True to knit surfaces, false to not; applies to mirroring surfaces only

Obsolete. Superseded by [IFeatureManager::InsertMirrorFeature2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeatureManager~InsertMirrorFeature2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertMirrorFeature( _    ByVal BMirrorBody As System.Boolean, _    ByVal BGeometryPattern As System.Boolean, _    ByVal BMerge As System.Boolean, _    ByVal BKnit As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim BMirrorBody As System.Boolean Dim BGeometryPattern As System.Boolean Dim BMerge As System.Boolean Dim BKnit As System.Boolean Dim value As Feature   value = instance.InsertMirrorFeature(BMirrorBody, BGeometryPattern, BMerge, BKnit) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertMirrorFeature(     System.bool BMirrorBody,    System.bool BGeometryPattern,    System.bool BMerge,    System.bool BKnit ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertMirrorFeature(  &   System.bool BMirrorBody, &   System.bool BGeometryPattern, &   System.bool BMerge, &   System.bool BKnit ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BMirrorBody*
:   True to mirror solid bodies; false to mirror a feature or face

*BGeometryPattern*
:   True to mirror only the feature geometry, false to solve the entire feature; applies
    to mirroring features only

*BMerge*
:   True to merge any mirrored solid bodies, false to not; applies to mirroring solid
    bodies only

*BKnit*
:   True to knit surfaces, false to not; applies to mirroring surfaces only

#### Return Value

Pointer to the [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertMirrorFeature.

# ![](dotnetimages/collapse.gif)Remarks

This method attempts to create the mirror feature without displaying a dialog box to get information from the user. It relies on preselected and marked entities, as well as arguments.

|  |  |
| --- | --- |
| **Any...** | **Must be preselected and marked with a value of...** |
| Features to be mirrored | 1 |
| Faces to be mirrored | 128 |
| Bodies to be mirrored | 256 |
| Plane or planar face | 2 |

For information on selecting and marking entities, see [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IMirrorSolidFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMirrorSolidFeatureData.html)

[IMirrorPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMirrorPatternFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0