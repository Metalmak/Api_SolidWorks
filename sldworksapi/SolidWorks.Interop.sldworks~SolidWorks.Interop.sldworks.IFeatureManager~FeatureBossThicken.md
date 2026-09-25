<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FeatureBossThicken.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureBossThicken Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : FeatureBossThicken Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Thickness*
:   Wall thickness

*Direction*
:   Direction as defined in swThickenThicknessType\_e

*FaceIndex*
:   Not used

*FillVolume*
:   True if you want to make a solid from the knitted surface, false if not (see **Remarks**)

*Merge*
:   True if you want to merge the results in a multibody part, false if not

*UseFeatScope*
:   True if the feature only affects selected bodies, false if the feature affects all bodies

*UseAutoSelect*
:   True to automatically select all bodies and have the feature affect those bodies, false to select the bodies the feature affects (see **Remarks**)

Thickens the selected reference surface, and then generates a boss.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FeatureBossThicken( _    ByVal Thickness As System.Double, _    ByVal Direction As System.Integer, _    ByVal FaceIndex As System.Integer, _    ByVal FillVolume As System.Boolean, _    ByVal Merge As System.Boolean, _    ByVal UseFeatScope As System.Boolean, _    ByVal UseAutoSelect As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Thickness As System.Double Dim Direction As System.Integer Dim FaceIndex As System.Integer Dim FillVolume As System.Boolean Dim Merge As System.Boolean Dim UseFeatScope As System.Boolean Dim UseAutoSelect As System.Boolean Dim value As Feature   value = instance.FeatureBossThicken(Thickness, Direction, FaceIndex, FillVolume, Merge, UseFeatScope, UseAutoSelect) ``` | |

| C# |  |
| --- | --- |
| ``` Feature FeatureBossThicken(     System.double Thickness,    System.int Direction,    System.int FaceIndex,    System.bool FillVolume,    System.bool Merge,    System.bool UseFeatScope,    System.bool UseAutoSelect ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ FeatureBossThicken(  &   System.double Thickness, &   System.int Direction, &   System.int FaceIndex, &   System.bool FillVolume, &   System.bool Merge, &   System.bool UseFeatScope, &   System.bool UseAutoSelect ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Thickness*
:   Wall thickness

*Direction*
:   Direction as defined in swThickenThicknessType\_e

*FaceIndex*
:   Not used

*FillVolume*
:   True if you want to make a solid from the knitted surface, false if not (see **Remarks**)

*Merge*
:   True if you want to merge the results in a multibody part, false if not

*UseFeatScope*
:   True if the feature only affects selected bodies, false if the feature affects all bodies

*UseAutoSelect*
:   True to automatically select all bodies and have the feature affect those bodies, false to select the bodies the feature affects (see **Remarks**)

#### Return Value

Pointer to the [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::FeatureBossThicken.

# ![](dotnetimages/collapse.gif)Example

[Create Thicken Feature (VBA)](Create_Thicken_Feature_Example_VB.htm)

[Fill Holes in Part (C#)](Fill_Holes_in_Part_Example_CSharp.htm)

[Fill Holes in Part (VB.NET)](Fill_Holes_in_Part_Example_VBNET.htm)

[Fill Holes in Part (VBA)](Fill_Holes_in_Part_Example_VB.htm)

[Thicken Surface and Generate Boss (VBA)](Thicken_Surface_and_Generate_Boss_Example_VB.htm)

[Thicken Surface and Generate Boss (VB.NET)](Thicken_Surface_and_Generate_Boss_Example_VBNET.htm)

[Thicken Surface and Generate Boss (C#)](Thicken_Surface_and_Generate_Boss_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method generates a boss feature by thickening a selected reference surface.  The surface must be selected with a mark of 1. See [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) for details.

If FillVolume is true, other arguments are ignored. A closed surface is required when FillVolume is true.

If UseAutoSelect is false, the user must select the bodies that the feature will affect.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IThickenFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData.html)

[IFeatureManager::FeatureCutThicken Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FeatureCutThicken.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0