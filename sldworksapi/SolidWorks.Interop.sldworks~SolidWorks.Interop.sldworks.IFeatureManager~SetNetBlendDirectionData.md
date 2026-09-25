<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~SetNetBlendDirectionData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetNetBlendDirectionData Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : SetNetBlendDirectionData Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Direction*
:   * 0 = Direction 1* 1 = Direction 2

*InfluenceType*
:   * 0 = Global* 1 = To Next Curve* 2 = To Next Sharp* 3 = To Next Edge

*TrimCurves*
:   * 0 = False to trim curves* 1 = True to trim curves

*BlendClosed*
:   True closes this boundary feature or boundary surface feature, false leaves this boundary feature or boundary surface feature open

*SplitSurfaces*
:   Not used

Sets the curve set data (one for each of the two directions) for this boundary feature or boundary surface feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetNetBlendDirectionData( _    ByVal Direction As System.Short, _    ByVal InfluenceType As System.Short, _    ByVal TrimCurves As System.Short, _    ByVal BlendClosed As System.Boolean, _    ByVal SplitSurfaces As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Direction As System.Short Dim InfluenceType As System.Short Dim TrimCurves As System.Short Dim BlendClosed As System.Boolean Dim SplitSurfaces As System.Boolean Dim value As Feature   value = instance.SetNetBlendDirectionData(Direction, InfluenceType, TrimCurves, BlendClosed, SplitSurfaces) ``` | |

| C# |  |
| --- | --- |
| ``` Feature SetNetBlendDirectionData(     System.short Direction,    System.short InfluenceType,    System.short TrimCurves,    System.bool BlendClosed,    System.bool SplitSurfaces ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ SetNetBlendDirectionData(  &   System.short Direction, &   System.short InfluenceType, &   System.short TrimCurves, &   System.bool BlendClosed, &   System.bool SplitSurfaces ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Direction*
:   * 0 = Direction 1* 1 = Direction 2

*InfluenceType*
:   * 0 = Global* 1 = To Next Curve* 2 = To Next Sharp* 3 = To Next Edge

*TrimCurves*
:   * 0 = False to trim curves* 1 = True to trim curves

*BlendClosed*
:   True closes this boundary feature or boundary surface feature, false leaves this boundary feature or boundary surface feature open

*SplitSurfaces*
:   Not used

#### Return Value

[Feature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::SetNetBlendDirectionData.

# ![](dotnetimages/collapse.gif)Example

[Insert Boundary Surface Feature (VBA)](Insert_Boundary_Surface_Feature_Example_VB.htm)

[Insert Boundary Feature (C#)](Insert_Boundary_Feature_Example_CSharp.htm)

[Insert Boundary Feature (VB.NET)](Insert_Boundary_Feature_Example_VBNET.htm)

[Insert Boundary Feature (VBA)](Insert_Boundary_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFeatureManager::InsertNetBlend Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertNetBlend.html)

[IFeatureManager::SetNetBlendCurveData Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~SetNetBlendCurveData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0