<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetForceOrTranslationValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetForceOrTranslationValues Method (ICWRemoteLoad) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html) : SetForceOrTranslationValues Method (ICWRemoteLoad) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BInclude*
:   1 to include force or translation in the remote load, 0 to not (see **Remarks**)

*BXValue*
:   1 to set the value in the x direction, 0 to not

*DXValue*
:   Force or translation in the x direction; valid only if BXValue = 1

*BYValue*
:   1 to set the value in the y direction, 0 to not

*DYValue*
:   Force or translation in the y direction; valid only if BYValue = 1

*BZValue*
:   1 to set the value in the z direction, 0 to not

*DZValue*
:   Force or translation in the z direction; valid only if BZValue = 1

Obsolete. Superseded by [ICWRemoteLoad::SetForceOrTranslationValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetForceOrTranslationValues2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetForceOrTranslationValues( _    ByVal BInclude As System.Integer, _    ByVal BXValue As System.Integer, _    ByVal DXValue As System.Double, _    ByVal BYValue As System.Integer, _    ByVal DYValue As System.Double, _    ByVal BZValue As System.Integer, _    ByVal DZValue As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRemoteLoad Dim BInclude As System.Integer Dim BXValue As System.Integer Dim DXValue As System.Double Dim BYValue As System.Integer Dim DYValue As System.Double Dim BZValue As System.Integer Dim DZValue As System.Double   instance.SetForceOrTranslationValues(BInclude, BXValue, DXValue, BYValue, DYValue, BZValue, DZValue) ``` | |

| C# |  |
| --- | --- |
| ``` void SetForceOrTranslationValues(     System.int BInclude,    System.int BXValue,    System.double DXValue,    System.int BYValue,    System.double DYValue,    System.int BZValue,    System.double DZValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetForceOrTranslationValues(  &   System.int BInclude, &   System.int BXValue, &   System.double DXValue, &   System.int BYValue, &   System.double DYValue, &   System.int BZValue, &   System.double DZValue ) ``` | |

#### Parameters

*BInclude*
:   1 to include force or translation in the remote load, 0 to not (see **Remarks**)

*BXValue*
:   1 to set the value in the x direction, 0 to not

*DXValue*
:   Force or translation in the x direction; valid only if BXValue = 1

*BYValue*
:   1 to set the value in the y direction, 0 to not

*DYValue*
:   Force or translation in the y direction; valid only if BYValue = 1

*BZValue*
:   1 to set the value in the z direction, 0 to not

*DZValue*
:   Force or translation in the z direction; valid only if BZValue = 1

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWRemoteLoad::SetForceOrTranslationValues.

# ![](dotnetimages/collapse.gif)Example

[Add a Remote Load with Distributed Coupling (VBA)](Add_Remote_Load_with_Distributed_Connection_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method is valid only if [ICWRemoteLoad::AllowDistributedCoupling](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~AllowDistributedCoupling.html) returns false (i.e., for frequency, buckling, nonlinear dynamic, or linear dynamic studies). If ICWRemoteLoad::AllowDistributedCoupling returns true (i.e., for linear static, topology, or nonlinear static studies), use [ICWRemoteLoad::SetForceOrTranslationValuesEx](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetForceOrTranslationValuesEx.html) instead of this method.

| This method sets components of ... | If [ICWRemoteLoad::LoadType](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWRemoteLoad~LoadType.html) is ... |
| --- | --- |
| Force | swsRemoteLoadType\_e.swsRemoteLoadType\_DirectLoad  - or -  swsRemoteLoadType\_e.swsRemoteLoadType\_RigidLoadOrMass |
| Translation | swsRemoteLoadType\_e.swsRemoteLoadType\_DirectDisplacement  - or -  swsRemoteLoadType\_e.swsRemoteLoadType\_RigidDisplacement |

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html)

[ICWRemoteLoad Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad_members.html)

[ICWRemoteLoad::GetForceOrTranslationValues Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~GetForceOrTranslationValues.html)

[ICWRemoteLoad::ForceOrTranslationUnit Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~ForceOrTranslationUnit.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0