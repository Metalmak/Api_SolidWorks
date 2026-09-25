<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertWrapFeature2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertWrapFeature2 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertWrapFeature2 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Type*
:   Type of wrap as defined in swWrapSketchType\_e

*Thickness*
:   Thickness; 0.00001 (thinnest) - 10000 (thickest)

*ReverseDir*
:   True to reverse the direction of the wrap, false to not

*Method*
:   Type of wrap method as defined in swWrapMethods\_e

*MeshFactor*
:   Accuracy of flattened triangle mesh; 1 (lowest) - 10 (highest)

Inserts a wrap feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertWrapFeature2( _    ByVal Type As System.Integer, _    ByVal Thickness As System.Double, _    ByVal ReverseDir As System.Boolean, _    ByVal Method As System.Integer, _    ByVal MeshFactor As System.Integer _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Type As System.Integer Dim Thickness As System.Double Dim ReverseDir As System.Boolean Dim Method As System.Integer Dim MeshFactor As System.Integer Dim value As Feature   value = instance.InsertWrapFeature2(Type, Thickness, ReverseDir, Method, MeshFactor) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertWrapFeature2(     System.int Type,    System.double Thickness,    System.bool ReverseDir,    System.int Method,    System.int MeshFactor ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertWrapFeature2(  &   System.int Type, &   System.double Thickness, &   System.bool ReverseDir, &   System.int Method, &   System.int MeshFactor ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Type*
:   Type of wrap as defined in swWrapSketchType\_e

*Thickness*
:   Thickness; 0.00001 (thinnest) - 10000 (thickest)

*ReverseDir*
:   True to reverse the direction of the wrap, false to not

*Method*
:   Type of wrap method as defined in swWrapMethods\_e

*MeshFactor*
:   Accuracy of flattened triangle mesh; 1 (lowest) - 10 (highest)

#### Return Value

Wrap [feature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertWrapFeature2.

# ![](dotnetimages/collapse.gif)Example

[Create Wrap Feature on Multiple Faces (C#)](Create_Wrap_Feature_on_Multiple_Faces_Example_CSharp.htm)

[Create Wrap Feature on Multiple Faces (VB.NET)](Create_Wrap_Feature_on_Multiple_Faces_Example_VBNET.htm)

[Create Wrap Feature on Multiple Faces (VBA)](Create_Wrap_Feature_on_Multiple_Faces_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

| To select... | Use [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) or [IModelDocExtension::SelectByRay](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByRay.html) and specify a Mark of... |
| --- | --- |
| One or more faces on which to place the wrap feature | 1 |
| Pull direction entity if Type is:   * swWrapSketchType\_e.swWrapSketchType\_Emboss - or -* swWrapSketchType\_e.swWrapSketchType\_Engrave   For a line or linear edge, the pull direction is the direction of the selected entity. For a plane, the pull direction is normal to the plane. To wrap the sketch normal to the sketch plane, do not select a pull direction entity. | 2 |
| 2D sketch containing no open contours; 3D sketches are not supported | 4 |

**NOTE:** The difference between this method and the now obsolete [IFeatureManager::InsertWrapFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertWrapFeature.html) is that IFeatureManager::InsertWrapFeature2 can create a wrap feature on one or more faces and IFeatureManager::InsertWrapFeature creates a wrap feature on one face only.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IWrapSketchFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IWrapSketchFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0