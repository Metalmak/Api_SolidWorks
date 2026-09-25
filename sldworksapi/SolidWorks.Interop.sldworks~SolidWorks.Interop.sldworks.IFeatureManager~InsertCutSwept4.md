<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertCutSwept4.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertCutSwept4 Method (IFeatureManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html) : InsertCutSwept4 Method (IFeatureManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Propagate*
:   True propagates the sweep cut to the next edge, false causes the sweep cut to occur only on the selected edge; to propagate to the next edge, the next edge must be tangent to the current edge

*Alignment*
:   If the curve used to sweep goes from one face to another or from one edge to another, then true causes the sweep to cut completely through the end faces of the cut, and false causes the cut to begin and end perpendicular to the sweep curve; therefore, it may not break through the two end faces of the body being cut

*TwistCtrlOption*
:   Twist control options as defined in swTwistControlType\_e

*KeepTangency*
:   If the sweep section has tangent segments, true causes the corresponding surfaces in the resulting sweep to be tangent, false does not

*BAdvancedSmoothing*
:   If the sweep section has circular or elliptical arcs, true approximates the sections and smooths the surfaces, false does not

*StartMatchingType*
:   Tangency type as defined in swTangencyType\_e

*EndMatchingType*
:   Tangency type as defined in swTangencyType\_e

*IsThinBody*
:   True if this feature is a thin body, false if not

*Thickness1*
:   Thickness value for the first direction

*Thickness2*
:   Thickness value for the second direction

*ThinType*
:   Thin wall type as defined in swThinWallType\_e

*PathAlign*
:   Align path type (see **Remarks**)

*UseFeatScope*
:   True if the feature only affects selected bodies, false if the feature affects all bodies

*UseAutoSelect*
:   True to automatically select all bodies and have the feature affect those bodies, false to select the bodies the feature affects (see Remarks)

*TwistAngle*
:   If TwistCtrlOption is set to swTwistControlType\_e.swTwistControlConstantTwistAlongPath, then specify end twist angle

*BMergeSmoothFaces*
:   True to merge smooth faces, false to not

*AssemblyFeatureScope*
:   True if the sweep cut affects only selected components in the assembly, false if the sweep cut affects all components in the assembly (**see Remarks**)

*AutoSelectComponents*
:   True to auto-select all affected components in the assembly, false to use manually selected components (**see Remarks**)

*PropagateFeatureToParts*
:   True to extend the sweep cut feature to all affected parts in the assembly, false to just insert the sweep cut into the assembly (**see Remarks**)

Obsolete. Superseded by [IFeatureManager::InsertCutSwept5](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertCutSwept5.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertCutSwept4( _    ByVal Propagate As System.Boolean, _    ByVal Alignment As System.Boolean, _    ByVal TwistCtrlOption As System.Short, _    ByVal KeepTangency As System.Boolean, _    ByVal BAdvancedSmoothing As System.Boolean, _    ByVal StartMatchingType As System.Short, _    ByVal EndMatchingType As System.Short, _    ByVal IsThinBody As System.Boolean, _    ByVal Thickness1 As System.Double, _    ByVal Thickness2 As System.Double, _    ByVal ThinType As System.Short, _    ByVal PathAlign As System.Short, _    ByVal UseFeatScope As System.Boolean, _    ByVal UseAutoSelect As System.Boolean, _    ByVal TwistAngle As System.Double, _    ByVal BMergeSmoothFaces As System.Boolean, _    ByVal AssemblyFeatureScope As System.Boolean, _    ByVal AutoSelectComponents As System.Boolean, _    ByVal PropagateFeatureToParts As System.Boolean _ ) As Feature ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFeatureManager Dim Propagate As System.Boolean Dim Alignment As System.Boolean Dim TwistCtrlOption As System.Short Dim KeepTangency As System.Boolean Dim BAdvancedSmoothing As System.Boolean Dim StartMatchingType As System.Short Dim EndMatchingType As System.Short Dim IsThinBody As System.Boolean Dim Thickness1 As System.Double Dim Thickness2 As System.Double Dim ThinType As System.Short Dim PathAlign As System.Short Dim UseFeatScope As System.Boolean Dim UseAutoSelect As System.Boolean Dim TwistAngle As System.Double Dim BMergeSmoothFaces As System.Boolean Dim AssemblyFeatureScope As System.Boolean Dim AutoSelectComponents As System.Boolean Dim PropagateFeatureToParts As System.Boolean Dim value As Feature   value = instance.InsertCutSwept4(Propagate, Alignment, TwistCtrlOption, KeepTangency, BAdvancedSmoothing, StartMatchingType, EndMatchingType, IsThinBody, Thickness1, Thickness2, ThinType, PathAlign, UseFeatScope, UseAutoSelect, TwistAngle, BMergeSmoothFaces, AssemblyFeatureScope, AutoSelectComponents, PropagateFeatureToParts) ``` | |

| C# |  |
| --- | --- |
| ``` Feature InsertCutSwept4(     System.bool Propagate,    System.bool Alignment,    System.short TwistCtrlOption,    System.bool KeepTangency,    System.bool BAdvancedSmoothing,    System.short StartMatchingType,    System.short EndMatchingType,    System.bool IsThinBody,    System.double Thickness1,    System.double Thickness2,    System.short ThinType,    System.short PathAlign,    System.bool UseFeatScope,    System.bool UseAutoSelect,    System.double TwistAngle,    System.bool BMergeSmoothFaces,    System.bool AssemblyFeatureScope,    System.bool AutoSelectComponents,    System.bool PropagateFeatureToParts ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Feature^ InsertCutSwept4(  &   System.bool Propagate, &   System.bool Alignment, &   System.short TwistCtrlOption, &   System.bool KeepTangency, &   System.bool BAdvancedSmoothing, &   System.short StartMatchingType, &   System.short EndMatchingType, &   System.bool IsThinBody, &   System.double Thickness1, &   System.double Thickness2, &   System.short ThinType, &   System.short PathAlign, &   System.bool UseFeatScope, &   System.bool UseAutoSelect, &   System.double TwistAngle, &   System.bool BMergeSmoothFaces, &   System.bool AssemblyFeatureScope, &   System.bool AutoSelectComponents, &   System.bool PropagateFeatureToParts ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Propagate*
:   True propagates the sweep cut to the next edge, false causes the sweep cut to occur only on the selected edge; to propagate to the next edge, the next edge must be tangent to the current edge

*Alignment*
:   If the curve used to sweep goes from one face to another or from one edge to another, then true causes the sweep to cut completely through the end faces of the cut, and false causes the cut to begin and end perpendicular to the sweep curve; therefore, it may not break through the two end faces of the body being cut

*TwistCtrlOption*
:   Twist control options as defined in swTwistControlType\_e

*KeepTangency*
:   If the sweep section has tangent segments, true causes the corresponding surfaces in the resulting sweep to be tangent, false does not

*BAdvancedSmoothing*
:   If the sweep section has circular or elliptical arcs, true approximates the sections and smooths the surfaces, false does not

*StartMatchingType*
:   Tangency type as defined in swTangencyType\_e

*EndMatchingType*
:   Tangency type as defined in swTangencyType\_e

*IsThinBody*
:   True if this feature is a thin body, false if not

*Thickness1*
:   Thickness value for the first direction

*Thickness2*
:   Thickness value for the second direction

*ThinType*
:   Thin wall type as defined in swThinWallType\_e

*PathAlign*
:   Align path type (see **Remarks**)

*UseFeatScope*
:   True if the feature only affects selected bodies, false if the feature affects all bodies

*UseAutoSelect*
:   True to automatically select all bodies and have the feature affect those bodies, false to select the bodies the feature affects (see Remarks)

*TwistAngle*
:   If TwistCtrlOption is set to swTwistControlType\_e.swTwistControlConstantTwistAlongPath, then specify end twist angle

*BMergeSmoothFaces*
:   True to merge smooth faces, false to not

*AssemblyFeatureScope*
:   True if the sweep cut affects only selected components in the assembly, false if the sweep cut affects all components in the assembly (**see Remarks**)

*AutoSelectComponents*
:   True to auto-select all affected components in the assembly, false to use manually selected components (**see Remarks**)

*PropagateFeatureToParts*
:   True to extend the sweep cut feature to all affected parts in the assembly, false to just insert the sweep cut into the assembly (**see Remarks**)

#### Return Value

Pointer to the [IFeature](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFeature.html) object

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See FeatureManager::InsertCutSwept4.

# ![](dotnetimages/collapse.gif)Example

[Insert Sweep Cut Feature (C#)](Insert_Sweep_Cut_Feature_Example_CSharp.htm)

[Insert Sweep Cut Feature (VB.NET)](Insert_Sweep_Cut_Feature_Example_VBNET.htm)

[Insert Sweep Cut Feature (VBA)](Insert_Sweep_Cut_Feature_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, call [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) multiple times to select the profile, guide curves, and sweep path for the cut, setting the Mark parameter in each case as follows:

* 1 = Profile selection

  * 2 = Guide-curve selection, if provided

    * 4 = Sweep path selection

The PathAlign argument is available when TwistCtrlOption is set to 0 and can take one of these values:

* 0 = None; no correction (default)

  * 2 = Direction vector; a plane, planar face, or line defines the path

    * 3 = All faces; includes neighboring faces

When UseAutoSelect is false, the user must select the bodies that the feature will affect.

When using cut or cavity features that result in multiple bodies, you cannot select to keep all of the resulting bodies or one or more selected bodies.

Use AssemblyFeatureScope, AutoSelectComponents, and PropagateFeatureToParts to insert sweep cuts into an assembly. AssemblyFeatureScope and AutoSelectComponents perform just like the configuration of the Feature Scope section on the PropertyManager page of the sweep feature:

| **AssemblyFeatureScope setting** | **AutoSelectComponents setting** | **PropertyManager page Feature Scope setting** |
| --- | --- | --- |
| False | Ignored | All components selected  Auto-select not visible |
| True | If true, affected components are automatically selected  If false, manually select the affected components in the view before calling this API | Selected components selected  If Auto-select is not seelcted, then manually select affected components in the view |

# ![](dotnetimages/collapse.gif)See Also

####

[IFeatureManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager.html)

[IFeatureManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager_members.html)

[ISweepFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweepFeatureData.html)

[IFeatureManager::InsertProtrusionSwept3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertProtrusionSwept3.html)

[IFeatureManager::InsertSweepSurface2 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeatureManager~InsertSweepSurface2.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0