<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetMomentOrRotationValues2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetMomentOrRotationValues2 Method (ICWRemoteLoad) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html) : SetMomentOrRotationValues2 Method (ICWRemoteLoad) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BInclude*
:   -1 or true to include moment or rotation in the remote load, 0 or false to not

*BXValue*
:   -1 or true to set the value in the x direction, 0 or false to not

*DXValue*
:   Moment or rotation in the x direction; valid only if BXValue = -1

*BYValue*
:   -1 or true to set the value in the y direction, 0 or false to not

*DYValue*
:   Moment or rotation in the y direction; valid only if BYValue = -1

*BZValue*
:   -1 or true to set the value in the z direction, 0 or false to not

*DZValue*
:   Moment or rotation in the z direction; valid only if BZValue = -1

Sets the components of moment or rotation for this remote load.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetMomentOrRotationValues2( _    ByVal BInclude As System.Boolean, _    ByVal BXValue As System.Boolean, _    ByVal DXValue As System.Double, _    ByVal BYValue As System.Boolean, _    ByVal DYValue As System.Double, _    ByVal BZValue As System.Boolean, _    ByVal DZValue As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRemoteLoad Dim BInclude As System.Boolean Dim BXValue As System.Boolean Dim DXValue As System.Double Dim BYValue As System.Boolean Dim DYValue As System.Double Dim BZValue As System.Boolean Dim DZValue As System.Double   instance.SetMomentOrRotationValues2(BInclude, BXValue, DXValue, BYValue, DYValue, BZValue, DZValue) ``` | |

| C# |  |
| --- | --- |
| ``` void SetMomentOrRotationValues2(     System.bool BInclude,    System.bool BXValue,    System.double DXValue,    System.bool BYValue,    System.double DYValue,    System.bool BZValue,    System.double DZValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetMomentOrRotationValues2(  &   System.bool BInclude, &   System.bool BXValue, &   System.double DXValue, &   System.bool BYValue, &   System.double DYValue, &   System.bool BZValue, &   System.double DZValue ) ``` | |

#### Parameters

*BInclude*
:   -1 or true to include moment or rotation in the remote load, 0 or false to not

*BXValue*
:   -1 or true to set the value in the x direction, 0 or false to not

*DXValue*
:   Moment or rotation in the x direction; valid only if BXValue = -1

*BYValue*
:   -1 or true to set the value in the y direction, 0 or false to not

*DYValue*
:   Moment or rotation in the y direction; valid only if BYValue = -1

*BZValue*
:   -1 or true to set the value in the z direction, 0 or false to not

*DZValue*
:   Moment or rotation in the z direction; valid only if BZValue = -1

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWRemoteLoad::AllowDistributedCoupling2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~AllowDistributedCoupling2.html) returns 0 or false (i.e., for frequency, buckling, nonlinear dynamic, or linear dynamic studies). If ICWRemoteLoad::AllowDistributedCoupling2 returns -1 or true (i.e., for linear static, topology, or nonlinear static studies), use [ICWRemoteLoad::SetMomentOrRotationValuesEx2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetMomentOrRotationValuesEx2.html) instead of this method.

| This method sets components of ... | If [ICWRemoteLoad::LoadType](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWRemoteLoad~LoadType.html) is ... |
| --- | --- |
| Moment | swsRemoteLoadType\_e.swsRemoteLoadType\_DirectLoad  - or -  swsRemoteLoadType\_e.swsRemoteLoadType\_RigidLoadOrMass |
| Rotation | swsRemoteLoadType\_e.swsRemoteLoadType\_RigidDisplacement  - or -  swsRemoteLoadType\_e.swsRemoteLoadType\_DirectDisplacement |

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html)

[ICWRemoteLoad Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30