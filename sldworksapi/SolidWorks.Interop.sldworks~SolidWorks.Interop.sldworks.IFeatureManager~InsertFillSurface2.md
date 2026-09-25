<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertFillSurface2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertFillSurface2 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertFillSurface2 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Resolutions*
:   Controls the resolution or quality of the surface (see **Remarks**)

*Options*
:   Options as defined in swFeatureFillSurfaceOptions\_e

*VPatchBoundaries*
:   Array of [edges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html) or [sketches](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch.html) for the patch boundaries

*VCurvatureControlType*
:   Array of curve control methods as defined in swContactType\_e

*VFaces*
:   Array of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) to use for direction

*VConstraintCurves*
:   Array of constraint curves ([edges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html) or [sketches](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch.html))

Inserts a fill-surface feature in the model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertFillSurface2( _    ByVal Resolutions As System.Integer, _    ByVal Options As System.Integer, _    ByVal VPatchBoundaries As System.Object, _    ByVal VCurvatureControlType As System.Object, _    ByVal VFaces As System.Object, _    ByVal VConstraintCurves As System.Object _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Resolutions As System.Integer Dim Options As System.Integer Dim VPatchBoundaries As System.Object Dim VCurvatureControlType As System.Object Dim VFaces As System.Object Dim VConstraintCurves As System.Object Dim value As Feature   value = instance.InsertFillSurface2(Resolutions, Options, VPatchBoundaries, VCurvatureControlType, VFaces, VConstraintCurves) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertFillSurface2(     System.int Resolutions,    System.int Options,    System.object VPatchBoundaries,    System.object VCurvatureControlType,    System.object VFaces,    System.object VConstraintCurves ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertFillSurface2(  &   System.int Resolutions, &   System.int Options, &   System.Object^ VPatchBoundaries, &   System.Object^ VCurvatureControlType, &   System.Object^ VFaces, &   System.Object^ VConstraintCurves ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Resolutions*
:   Controls the resolution or quality of the surface (see **Remarks**)

*Options*
:   Options as defined in swFeatureFillSurfaceOptions\_e

*VPatchBoundaries*
:   Array of [edges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html) or [sketches](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch.html) for the patch boundaries

*VCurvatureControlType*
:   Array of curve control methods as defined in swContactType\_e

*VFaces*
:   Array of [faces](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2.html) to use for direction

*VConstraintCurves*
:   Array of constraint curves ([edges](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IEdge.html) or [sketches](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketch.html))

#### Return Value

Pointer to the [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertFillSurface2.

# ![](dotnetimages/collapse.gif)Example

[Insert Fill-surface Feature (C#)](Insert_Fill-surface_Feature_Example_CSharp.htm)

[Insert Fill-surface Feature (VB.NET)](Insert_Fill-surface_Feature_Example_VBNET.htm)

[Insert Fill-surface Feature (VBA)](Insert_Fill-surface_Feature_Example_VB.htm)

[Get and Fill Gaps in Body (C#)](Get_and_Fill_Gaps_in_Body_Example_CSharp.htm)

[Get and Fill Gaps in Body (VB.NET)](Get_and_Fill_Gaps_in_Body_Example_VBNET.htm)

[Get and Fill Gaps in Body (VBA)](Get_and_Fill_Gaps_in_Body_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

You must use [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) and the following Mark values to select edges that bound the surface to be filled:

* Boundary curves = 1

  * Boundary with contact curvature control = 257

    * Boundary with tangent curvature control = 513

      * Constraint curves or internal curves = 4

The resolution argument can be set to 1, 2, or 3. The higher the value, the better the resolution.

Use the [IBody2::Diagnose](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IBody2~Diagnose.html) and the [IDiagnoseResult](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IDiagnoseResult.html) APIs to get the gaps to fill.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFillSurfaceFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFillSurfaceFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0