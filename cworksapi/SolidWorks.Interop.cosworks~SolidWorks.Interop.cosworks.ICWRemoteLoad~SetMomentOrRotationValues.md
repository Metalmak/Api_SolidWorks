<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetMomentOrRotationValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetMomentOrRotationValues Method (ICWRemoteLoad) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html) : SetMomentOrRotationValues Method (ICWRemoteLoad) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BInclude*
:   1 to include moment or rotation in the remote load, 0 to not

*BXValue*
:   1 to set the value in the x direction, 0 to not

*DXValue*
:   Moment or rotation in the x direction; valid only if BXValue = 1

*BYValue*
:   1 to set the value in the y direction, 0 to not

*DYValue*
:   Moment or rotation in the y direction; valid only if BYValue = 1

*BZValue*
:   1 to set the value in the z direction, 0 to not

*DZValue*
:   Moment or rotation in the z direction; valid only if BZValue = 1

Obsolete. Superseded by [ICWRemoteLoad::SetMomentOrRotationValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetMomentOrRotationValues2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetMomentOrRotationValues( _    ByVal BInclude As System.Integer, _    ByVal BXValue As System.Integer, _    ByVal DXValue As System.Double, _    ByVal BYValue As System.Integer, _    ByVal DYValue As System.Double, _    ByVal BZValue As System.Integer, _    ByVal DZValue As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRemoteLoad Dim BInclude As System.Integer Dim BXValue As System.Integer Dim DXValue As System.Double Dim BYValue As System.Integer Dim DYValue As System.Double Dim BZValue As System.Integer Dim DZValue As System.Double   instance.SetMomentOrRotationValues(BInclude, BXValue, DXValue, BYValue, DYValue, BZValue, DZValue) ``` | |

| C# |  |
| --- | --- |
| ``` void SetMomentOrRotationValues(     System.int BInclude,    System.int BXValue,    System.double DXValue,    System.int BYValue,    System.double DYValue,    System.int BZValue,    System.double DZValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetMomentOrRotationValues(  &   System.int BInclude, &   System.int BXValue, &   System.double DXValue, &   System.int BYValue, &   System.double DYValue, &   System.int BZValue, &   System.double DZValue ) ``` | |

#### Parameters

*BInclude*
:   1 to include moment or rotation in the remote load, 0 to not

*BXValue*
:   1 to set the value in the x direction, 0 to not

*DXValue*
:   Moment or rotation in the x direction; valid only if BXValue = 1

*BYValue*
:   1 to set the value in the y direction, 0 to not

*DYValue*
:   Moment or rotation in the y direction; valid only if BYValue = 1

*BZValue*
:   1 to set the value in the z direction, 0 to not

*DZValue*
:   Moment or rotation in the z direction; valid only if BZValue = 1

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWRemoteLoad::SetMomentOrRotationValues.

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWRemoteLoad::AllowDistributedCoupling](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~AllowDistributedCoupling.html) returns false (i.e., for frequency, buckling, nonlinear dynamic, or linear dynamic studies). If ICWRemoteLoad::AllowDistributedCoupling returns true (i.e., for linear static, topology, or nonlinear static studies), use [ICWRemoteLoad::SetMomentOrRotationValuesEx](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetMomentOrRotationValuesEx.html) instead of this method.

| This method sets components of ... | If [ICWRemoteLoad::LoadType](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWRemoteLoad~LoadType.html) is ... |
| --- | --- |
| Moment | swsRemoteLoadType\_e.swsRemoteLoadType\_DirectLoad  - or -  swsRemoteLoadType\_e.swsRemoteLoadType\_RigidLoadOrMass |
| Rotation | swsRemoteLoadType\_e.swsRemoteLoadType\_RigidDisplacement  - or -  swsRemoteLoadType\_e.swsRemoteLoadType\_DirectDisplacement |

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html)

[ICWRemoteLoad Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad_members.html)

[ICWRemoteLoad::GetMomentOrRotationValues Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~GetMomentOrRotationValues.html)

[ICWRemoteLoad::MomentOrRotationUnit Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~MomentOrRotationUnit.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0