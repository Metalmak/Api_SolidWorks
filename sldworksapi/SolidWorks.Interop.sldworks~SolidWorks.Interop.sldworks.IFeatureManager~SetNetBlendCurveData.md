<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~SetNetBlendCurveData.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetNetBlendCurveData Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : SetNetBlendCurveData Method (IFeatureManager) |

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

*CurveIndex*
:   Index of curve in the specified direction

*TangentType*
:   Type of tangency as defined in swTangencyType\_e

*SignedDraftAngle*
:   Draft angle

*SignedTangentLength*
:   Tangent length

*TangentLengthApplyAll*
:   True if the tangent length applies to all curves, false if not

Sets the data for a curve for this boundary feature or boundary surface feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetNetBlendCurveData( _    ByVal Direction As System.Short, _    ByVal CurveIndex As System.Short, _    ByVal TangentType As System.Short, _    ByVal SignedDraftAngle As System.Double, _    ByVal SignedTangentLength As System.Double, _    ByVal TangentLengthApplyAll As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Direction As System.Short Dim CurveIndex As System.Short Dim TangentType As System.Short Dim SignedDraftAngle As System.Double Dim SignedTangentLength As System.Double Dim TangentLengthApplyAll As System.Boolean Dim value As Feature   value = instance.SetNetBlendCurveData(Direction, CurveIndex, TangentType, SignedDraftAngle, SignedTangentLength, TangentLengthApplyAll) ``` | |

| C# |  |
| --- | --- |
| ``` Feature SetNetBlendCurveData(     System.short Direction,    System.short CurveIndex,    System.short TangentType,    System.double SignedDraftAngle,    System.double SignedTangentLength,    System.bool TangentLengthApplyAll ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ SetNetBlendCurveData(  &   System.short Direction, &   System.short CurveIndex, &   System.short TangentType, &   System.double SignedDraftAngle, &   System.double SignedTangentLength, &   System.bool TangentLengthApplyAll ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Direction*
:   * 0 = Direction 1* 1 = Direction 2

*CurveIndex*
:   Index of curve in the specified direction

*TangentType*
:   Type of tangency as defined in swTangencyType\_e

*SignedDraftAngle*
:   Draft angle

*SignedTangentLength*
:   Tangent length

*TangentLengthApplyAll*
:   True if the tangent length applies to all curves, false if not

#### Return Value

[Feature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::SetNetBlendCurveData.

# ![](dotnetimages/collapse.gif)Example

[Insert Boundary Surface Feature (VBA)](Insert_Boundary_Surface_Feature_Example_VB.htm)

[Insert Boundary Feature (C#)](Insert_Boundary_Feature_Example_CSharp.htm)

[Insert Boundary Feature (VB.NET)](Insert_Boundary_Feature_Example_VBNET.htm)

[Insert Boundary Feature (VBA)](Insert_Boundary_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

You must use this method to set the data for each curve in a boundary feature or boundary surface feature.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[IFeatureManager::InsertNetBlend Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertNetBlend.html)

[IFeatureManager::SetNetBlendDirectionData Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~SetNetBlendDirectionData.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0