<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~PreTrimSurface.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| PreTrimSurface Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : PreTrimSurface Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BMutualTrimIn*
:   True to use the selected intersecting surfaces as the trimming surfaces (mutual), false to use the selected surface, plane, or sketch as the trim tool (standard)

*BSplitSystemIn*
:   True to let the SOLIDWORKS application determine which surfaces to trim, false to trim all possible surfaces

*BSplitLinearIn*
:   False to naturally extend any trims along the intersecting surfaces, true to extend any trims linearly along the intersecting surfaces

*BRemovePickedIn*
:   True to remove the selected surfaces, false to keep the selected surfaces

Sets the trimming options before trimming a surface.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function PreTrimSurface( _    ByVal BMutualTrimIn As System.Boolean, _    ByVal BSplitSystemIn As System.Boolean, _    ByVal BSplitLinearIn As System.Boolean, _    ByVal BRemovePickedIn As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim BMutualTrimIn As System.Boolean Dim BSplitSystemIn As System.Boolean Dim BSplitLinearIn As System.Boolean Dim BRemovePickedIn As System.Boolean Dim value As System.Boolean   value = instance.PreTrimSurface(BMutualTrimIn, BSplitSystemIn, BSplitLinearIn, BRemovePickedIn) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool PreTrimSurface(     System.bool BMutualTrimIn,    System.bool BSplitSystemIn,    System.bool BSplitLinearIn,    System.bool BRemovePickedIn ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool PreTrimSurface(  &   System.bool BMutualTrimIn, &   System.bool BSplitSystemIn, &   System.bool BSplitLinearIn, &   System.bool BRemovePickedIn ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*BMutualTrimIn*
:   True to use the selected intersecting surfaces as the trimming surfaces (mutual), false to use the selected surface, plane, or sketch as the trim tool (standard)

*BSplitSystemIn*
:   True to let the SOLIDWORKS application determine which surfaces to trim, false to trim all possible surfaces

*BSplitLinearIn*
:   False to naturally extend any trims along the intersecting surfaces, true to extend any trims linearly along the intersecting surfaces

*BRemovePickedIn*
:   True to remove the selected surfaces, false to keep the selected surfaces

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::PreTrimSurface.

# ![](dotnetimages/collapse.gif)Example

[Create Trimmed Surface Feature (C#)](Create_Trimmed_Surface_Feature_Example_CSharp.htm)

[Create Trimmed Surface Feature (VB.NET)](Create_Trimmed_Surface_Feature_Example_VBNET.htm)

[Create Trimmed Surface Feature (VBA)](Create_Trimmed_Surface_Feature_Example_VB.htm)

[Create Solid Body Surface Trim Feature (C#)](Create_Solid_Body_Surface_Trim_Feature_Example_CSharp.htm)

[Create Solid Body Surface Trim Feature (VB.NET)](Create_Solid_Body_Surface_Trim_Feature_Example_VBNET.htm)

[Create Solid Body Surface Trim Feature (VBA)](Create_Solid_Body_Surface_Trim_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

After calling this method:

1. Select the trimming surfaces or trim tool.- Optionally, call [IFeatureManager::SolidForTrim](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~SolidForTrim.html).- Call [IFeatureManager::PostTrimSurface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~PostTrimSurface.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[ISurfaceTrimFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISurfaceTrimFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12.0