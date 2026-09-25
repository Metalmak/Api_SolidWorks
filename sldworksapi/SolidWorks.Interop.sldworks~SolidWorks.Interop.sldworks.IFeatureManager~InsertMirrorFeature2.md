<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertMirrorFeature2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertMirrorFeature2 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertMirrorFeature2 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BMirrorBody*
:   True to mirror solid bodies; false to mirror a feature or face

*BGeometryPattern*
:   True to mirror only the feature geometry, false to solve the entire feature; applies to mirroring features only

*BMerge*
:   True to merge any mirrored solid bodies, false to not; applies to mirroring solid bodies only

*BKnit*
:   True to knit surfaces, false to not; applies to mirroring surfaces only

*ScopeOptions*
:   Feature scope as defined by swFeatureScope\_e

Mirrors selected features, faces, and bodies about a selected plane or planar face.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertMirrorFeature2( _    ByVal BMirrorBody As System.Boolean, _    ByVal BGeometryPattern As System.Boolean, _    ByVal BMerge As System.Boolean, _    ByVal BKnit As System.Boolean, _    ByVal ScopeOptions As System.Integer _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim BMirrorBody As System.Boolean Dim BGeometryPattern As System.Boolean Dim BMerge As System.Boolean Dim BKnit As System.Boolean Dim ScopeOptions As System.Integer Dim value As Feature   value = instance.InsertMirrorFeature2(BMirrorBody, BGeometryPattern, BMerge, BKnit, ScopeOptions) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertMirrorFeature2(     System.bool BMirrorBody,    System.bool BGeometryPattern,    System.bool BMerge,    System.bool BKnit,    System.int ScopeOptions ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertMirrorFeature2(  &   System.bool BMirrorBody, &   System.bool BGeometryPattern, &   System.bool BMerge, &   System.bool BKnit, &   System.int ScopeOptions ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BMirrorBody*
:   True to mirror solid bodies; false to mirror a feature or face

*BGeometryPattern*
:   True to mirror only the feature geometry, false to solve the entire feature; applies to mirroring features only

*BMerge*
:   True to merge any mirrored solid bodies, false to not; applies to mirroring solid bodies only

*BKnit*
:   True to knit surfaces, false to not; applies to mirroring surfaces only

*ScopeOptions*
:   Feature scope as defined by swFeatureScope\_e

#### Return Value

[Feature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertMirrorFeature2.

# ![](dotnetimages/collapse.gif)Example

[Get Mirror Pattern Feature Data (C#)](Get_Mirror_Pattern_Feature_Data_Example_CSharp.htm)

[Get Mirror Pattern Feature Data (VB.NET)](Get_Mirror_Pattern_Feature_Data_Example_VBNET.htm)

[Get Mirror Pattern Feature Data (VBA)](Get_Mirror_Feature_Data_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method attempts to create the mirror feature without displaying a dialog box to get information from the user. It relies on preselected and marked entities and arguments.

|  |  |
| --- | --- |
| **Any...** | **Must be preselected and marked with a value of...** |
| Features to be mirrored | 1 |
| Faces to be mirrored | 128 |
| Bodies to be mirrored | 256 |
| Plane or planar face | 2 |

For information on selecting and marking entities, see [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IMirrorPatternFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMirrorPatternFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0