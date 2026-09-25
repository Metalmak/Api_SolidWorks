<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertSweepSurface2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertSweepSurface2 Method (IFeatureManager) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertSweepSurface2 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Propagate*
:   True propagates the sweep to the next edge, false causes the sweep to occur only on the selected edge; to propagate to the next edge, the next edge must be tangent to the current edge

*TwistCtrlOption*
:   Twist control option as defined in swTwistControlType\_e

*KeepTangency*
:   If the sweep section has tangent segments, then true to cause the corresponding surfaces in the resulting sweep to be tangent, false to not

*BAdvancedSmoothing*
:   If the sweep section has circular or elliptical arcs, then true to approximate the sections and smooth the surfaces, false to not

*StartMatchingType*
:   Tangency type as defined in swTangencyType\_e

*EndMatchingType*
:   Tangency type as defined in swTangencyType\_e

*PathAlign*
:   Align path type (see **Remarks**)

*UseFeatScope*
:   True if the feature only affects selected bodies, false if the feature affects all bodies

*UseAutoSelect*
:   True to automatically select all bodies and have the feature affect those bodies, false to select the bodies the feature affects (see **Remarks**)

*TwistAngle*
:   If TwistCtrlOption set to swTwistControlType\_e.swTwistControlConstantTwistAlongPath, then specify end twist angle

*BMergeSmoothFaces*
:   True to merge smooth faces, false to not

Obsolete. Superseded by [IFeatureManager::InsertSweepSurface3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertSweepSurface3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertSweepSurface2( _    ByVal Propagate As System.Boolean, _    ByVal TwistCtrlOption As System.Short, _    ByVal KeepTangency As System.Boolean, _    ByVal BAdvancedSmoothing As System.Boolean, _    ByVal StartMatchingType As System.Short, _    ByVal EndMatchingType As System.Short, _    ByVal PathAlign As System.Short, _    ByVal UseFeatScope As System.Boolean, _    ByVal UseAutoSelect As System.Boolean, _    ByVal TwistAngle As System.Double, _    ByVal BMergeSmoothFaces As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Propagate As System.Boolean Dim TwistCtrlOption As System.Short Dim KeepTangency As System.Boolean Dim BAdvancedSmoothing As System.Boolean Dim StartMatchingType As System.Short Dim EndMatchingType As System.Short Dim PathAlign As System.Short Dim UseFeatScope As System.Boolean Dim UseAutoSelect As System.Boolean Dim TwistAngle As System.Double Dim BMergeSmoothFaces As System.Boolean Dim value As Feature   value = instance.InsertSweepSurface2(Propagate, TwistCtrlOption, KeepTangency, BAdvancedSmoothing, StartMatchingType, EndMatchingType, PathAlign, UseFeatScope, UseAutoSelect, TwistAngle, BMergeSmoothFaces) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertSweepSurface2(     System.bool Propagate,    System.short TwistCtrlOption,    System.bool KeepTangency,    System.bool BAdvancedSmoothing,    System.short StartMatchingType,    System.short EndMatchingType,    System.short PathAlign,    System.bool UseFeatScope,    System.bool UseAutoSelect,    System.double TwistAngle,    System.bool BMergeSmoothFaces ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertSweepSurface2(  &   System.bool Propagate, &   System.short TwistCtrlOption, &   System.bool KeepTangency, &   System.bool BAdvancedSmoothing, &   System.short StartMatchingType, &   System.short EndMatchingType, &   System.short PathAlign, &   System.bool UseFeatScope, &   System.bool UseAutoSelect, &   System.double TwistAngle, &   System.bool BMergeSmoothFaces ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Propagate*
:   True propagates the sweep to the next edge, false causes the sweep to occur only on the selected edge; to propagate to the next edge, the next edge must be tangent to the current edge

*TwistCtrlOption*
:   Twist control option as defined in swTwistControlType\_e

*KeepTangency*
:   If the sweep section has tangent segments, then true to cause the corresponding surfaces in the resulting sweep to be tangent, false to not

*BAdvancedSmoothing*
:   If the sweep section has circular or elliptical arcs, then true to approximate the sections and smooth the surfaces, false to not

*StartMatchingType*
:   Tangency type as defined in swTangencyType\_e

*EndMatchingType*
:   Tangency type as defined in swTangencyType\_e

*PathAlign*
:   Align path type (see **Remarks**)

*UseFeatScope*
:   True if the feature only affects selected bodies, false if the feature affects all bodies

*UseAutoSelect*
:   True to automatically select all bodies and have the feature affect those bodies, false to select the bodies the feature affects (see **Remarks**)

*TwistAngle*
:   If TwistCtrlOption set to swTwistControlType\_e.swTwistControlConstantTwistAlongPath, then specify end twist angle

*BMergeSmoothFaces*
:   True to merge smooth faces, false to not

#### Return Value

Pointer to the [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertSweepSurface2.

# ![](dotnetimages/collapse.gif)Remarks

Because you are creating a surface, the sections can be open.

Use [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) to select the profile and sweep curves. The mark for:

* 1 = Profile selection

  * 2 = Guide curve selection, if provided

    * 4 = Sweep path

The PathAlign argument is available when TwistCtrlOption is set to swTwistControlFollowPath and can take one of these values:

* 0 = None; no correction (default)

  * 2 = Direction vector; a plane, planar face, or line defines the path

    * 3 = All faces; includes neighboring faces

When UseAutoSelect is false, the user must select the bodies that the feature will affect.

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0