<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~GetMomentOrRotationValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetMomentOrRotationValues Method (ICWRemoteLoad) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html) : GetMomentOrRotationValues Method (ICWRemoteLoad) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BInclude*
:   1 to get moment or rotation values, 0 to not (see **Remarks**)

*BXValue*
:   1 to get the value in the x direction, 0 to not

*DXValue*
:   Moment or rotation in the x direction; valid only if BXValue = 1

*BYValue*
:   1 to get the value in the y direction, 0 to not

*DYValue*
:   Moment or rotation in the y direction; valid only if BYValue = 1

*BZValue*
:   1 to get the value in the z direction, 0 to not

*DZValue*
:   Moment or rotation in the z direction; valid only if BZValue = 1

Obsolete. Superseded by [ICWRemoteLoad::GetMomentOrRotationValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~GetMomentOrRotationValues2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetMomentOrRotationValues( _    ByRef BInclude As System.Integer, _    ByRef BXValue As System.Integer, _    ByRef DXValue As System.Double, _    ByRef BYValue As System.Integer, _    ByRef DYValue As System.Double, _    ByRef BZValue As System.Integer, _    ByRef DZValue As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRemoteLoad Dim BInclude As System.Integer Dim BXValue As System.Integer Dim DXValue As System.Double Dim BYValue As System.Integer Dim DYValue As System.Double Dim BZValue As System.Integer Dim DZValue As System.Double   instance.GetMomentOrRotationValues(BInclude, BXValue, DXValue, BYValue, DYValue, BZValue, DZValue) ``` | |

| C# |  |
| --- | --- |
| ``` void GetMomentOrRotationValues(     out System.int BInclude,    out System.int BXValue,    out System.double DXValue,    out System.int BYValue,    out System.double DYValue,    out System.int BZValue,    out System.double DZValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetMomentOrRotationValues(  &   [Out] System.int BInclude, &   [Out] System.int BXValue, &   [Out] System.double DXValue, &   [Out] System.int BYValue, &   [Out] System.double DYValue, &   [Out] System.int BZValue, &   [Out] System.double DZValue ) ``` | |

#### Parameters

*BInclude*
:   1 to get moment or rotation values, 0 to not (see **Remarks**)

*BXValue*
:   1 to get the value in the x direction, 0 to not

*DXValue*
:   Moment or rotation in the x direction; valid only if BXValue = 1

*BYValue*
:   1 to get the value in the y direction, 0 to not

*DYValue*
:   Moment or rotation in the y direction; valid only if BYValue = 1

*BZValue*
:   1 to get the value in the z direction, 0 to not

*DZValue*
:   Moment or rotation in the z direction; valid only if BZValue = 1

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWRemoteLoad::GetMomentOrRotationValues.

# ![](dotnetimages/collapse.gif)Remarks

| This method gets components of ... | If [ICWRemoteLoad::LoadType](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWRemoteLoad~LoadType.html) is ... |
| --- | --- |
| Moment | swsRemoteLoadType\_e.swsRemoteLoadType\_DirectLoad  - or -  swsRemoteLoadType\_e.swsRemoteLoadType\_RigidLoadOrMass |
| Rotation | swsRemoteLoadType\_e.swsRemoteLoadType\_RigidDisplacement  - or -  swsRemoteLoadType\_e.swsRemoteLoadType\_DirectDisplacement |

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html)

[ICWRemoteLoad Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad_members.html)

[ICWRemoteLoad::SetMomentOrRotationValues Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetMomentOrRotationValues.html)

[ICWRemoteLoad::MomentOrRotationUnit Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~MomentOrRotationUnit.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0