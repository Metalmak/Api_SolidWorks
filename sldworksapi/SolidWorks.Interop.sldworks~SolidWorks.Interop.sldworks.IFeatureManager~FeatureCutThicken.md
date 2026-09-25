<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FeatureCutThicken.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| FeatureCutThicken Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : FeatureCutThicken Method (IFeatureManager) |

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
:   * 0 = Thicken side 1

      * 1 = Thicken side 2

        * 2 = Thicken both sides

*FaceIndex*
:   Not currently used

*FillVolume*
:   True to make the solid from a knitted surface, false to not (see **Remarks**)

*UseFeatScope*
:   True if the feature only affects selected bodies, false if the feature affects all bodies

*UseAutoSelect*
:   True to automatically select all bodies and have the feature affect  those bodies, false to select the bodies the feature affects (see Remarks)

Thickens the selected reference surface feature, and then generates a cut.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function FeatureCutThicken( _    ByVal Thickness As System.Double, _    ByVal Direction As System.Integer, _    ByVal FaceIndex As System.Integer, _    ByVal FillVolume As System.Boolean, _    ByVal UseFeatScope As System.Boolean, _    ByVal UseAutoSelect As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Thickness As System.Double Dim Direction As System.Integer Dim FaceIndex As System.Integer Dim FillVolume As System.Boolean Dim UseFeatScope As System.Boolean Dim UseAutoSelect As System.Boolean Dim value As Feature   value = instance.FeatureCutThicken(Thickness, Direction, FaceIndex, FillVolume, UseFeatScope, UseAutoSelect) ``` | |

| C# |  |
| --- | --- |
| ``` Feature FeatureCutThicken(     System.double Thickness,    System.int Direction,    System.int FaceIndex,    System.bool FillVolume,    System.bool UseFeatScope,    System.bool UseAutoSelect ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ FeatureCutThicken(  &   System.double Thickness, &   System.int Direction, &   System.int FaceIndex, &   System.bool FillVolume, &   System.bool UseFeatScope, &   System.bool UseAutoSelect ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Thickness*
:   Wall thickness

*Direction*
:   * 0 = Thicken side 1

      * 1 = Thicken side 2

        * 2 = Thicken both sides

*FaceIndex*
:   Not currently used

*FillVolume*
:   True to make the solid from a knitted surface, false to not (see **Remarks**)

*UseFeatScope*
:   True if the feature only affects selected bodies, false if the feature affects all bodies

*UseAutoSelect*
:   True to automatically select all bodies and have the feature affect  those bodies, false to select the bodies the feature affects (see Remarks)

#### Return Value

Pointer to the [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::FeatureCutThicken.

# ![](dotnetimages/collapse.gif)Remarks

This method creates a cut feature by thickening a selected reference surface. If FillVolume is True, other arguments are ignored. A closed surface is required when FillVolume is True.

When UseAutoSelect is false, the user must select the bodies that the feature will affect.

When using cut or cavity features that result in multiple bodies, you cannot select to keep all of the resulting bodies or one or more selected bodies.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFeatureManager::FeatureCut2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FeatureCut2.html)

[IFeatureManager::FeatureCutThin Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FeatureCutThin.html)

[IFeatureManager::FeatureBossThicken Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~FeatureBossThicken.html)

[IThickenFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IThickenFeatureData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0