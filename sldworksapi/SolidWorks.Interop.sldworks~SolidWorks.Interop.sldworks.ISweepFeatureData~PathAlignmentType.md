<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweepFeatureData~PathAlignmentType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| PathAlignmentType Property (ISweepFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISweepFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweepFeatureData.html) : PathAlignmentType Property (ISweepFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the alignment of the sweep path in this sweep feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property PathAlignmentType As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISweepFeatureData Dim value As System.Integer   instance.PathAlignmentType = value   value = instance.PathAlignmentType ``` | |

| C# |  |
| --- | --- |
| ``` System.int PathAlignmentType {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int PathAlignmentType {    System.int get();    void set ( &   System.int value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

Sweep path alignment as defined in swTangencyType\_e:

* swTangencyAllFaces* swTangencyDirectionVector* swTangencyNone

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SweepFeatureData::PathAlignmentType.

# ![](dotnetimages/collapse.gif)Example

See the [ISweepFeatureData](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweepFeatureData.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

| For user interface option... | | Set... | |
| --- | --- | --- | --- |
| **Profile Orientation set to...** | **And Profile Twist set to...** | **[ISweepFeatureData::TwistControlType](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweepFeatureData~TwistControlType.html) as defined in swTwistControlType\_e to...** | **And** **ISweepFeatureData::PathAlignmentType** **as defined in swTangencyType\_e to...** |
| Follow Path | None | swTwistControlFollowPath | swTangencyNone |
| Specify Twist Value | swTwistControlConstantTwistAlongPath | swTangencyNone |
| Specify Direction Vector | swTwistControlFollowPath | swTangencyDirectionVector; call [ISweepFeatureData::SetPathAlignmentDirectionVector](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweepFeatureData~SetPathAlignmentDirectionVector.html) to specify the direction vector |
| Follow Path and First Guide Curve (option appears with at least one guide curve) | swTwistControlFollowPathFirstGuideCurve | swTangencyNone |
| Follow Path and First and Second Guide Curves (option appears with at least two guide curves) | swTwistControlFollowFirstSecondGuideCurves | swTangencyNone |
| Tangent to Adjacent Faces | swTwistControlFollowPath | swTangencyAllFaces |
| Minimum Twist (available only with a 3D path) | swTwistControlFollowPath | swMinimumTwist |
| Natural | swTwistControlFollowPath | swTangencyNone |
| Keep Normal Constant | None | swTwistControlKeepNormalConstant | swTangencyNone |
| Specify Twist Value | swTwistControlConstantTwistAlongPath + swTwistControlKeepNormalConstant | swTangencyNone |

See Accessing Selections that Define Features for additional details.

# ![](dotnetimages/collapse.gif)See Also

####

[ISweepFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweepFeatureData.html)

[ISweepFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweepFeatureData_members.html)

[ISweepFeatureData::GetPathAlignmentDirectionVector Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweepFeatureData~GetPathAlignmentDirectionVector.html)

[ISweepFeatureData::GetPathType Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISweepFeatureData~GetPathType.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 FCS, Revision Number 13.0