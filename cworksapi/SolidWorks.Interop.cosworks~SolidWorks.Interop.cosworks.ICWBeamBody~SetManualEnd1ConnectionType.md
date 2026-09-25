<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~SetManualEnd1ConnectionType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetManualEnd1ConnectionType Method (ICWBeamBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWBeamBody Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody.html) : SetManualEnd1ConnectionType Method (ICWBeamBody) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BHingeIstDir*
:   1 to set the moment about the first direction of the cross section to zero so that the end can rotate about this direction, 0 to not

*BHinge2ndDir*
:   1 to set the moment about the second direction of the cross section to zero so that the end can rotate about this direction, 0 to not

*BHingeAlongBeam*
:   1 to set the moment about the axial direction of the beam to zero so that the end can rotate about this direction, 0 to not

*BSlide1stDir*
:   1 to set the force in the first direction of the cross section to zero so that the end can translate along this direction, 0 to not

*BSlide2ndDir*
:   1 to set the force in the second direction of the cross section to zero so that the end can translate along this direction, 0 to not

*BSlideAlongBeam*
:   1 to set the force in the axial direction of the beam to zero so that the end can translate along this direction, 0 to not

Obsolete. Superseded by [ICWBeamBody::SetManualEnd1ConnectionType2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~SetManualEnd1ConnectionType2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetManualEnd1ConnectionType( _    ByVal BHingeIstDir As System.Integer, _    ByVal BHinge2ndDir As System.Integer, _    ByVal BHingeAlongBeam As System.Integer, _    ByVal BSlide1stDir As System.Integer, _    ByVal BSlide2ndDir As System.Integer, _    ByVal BSlideAlongBeam As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWBeamBody Dim BHingeIstDir As System.Integer Dim BHinge2ndDir As System.Integer Dim BHingeAlongBeam As System.Integer Dim BSlide1stDir As System.Integer Dim BSlide2ndDir As System.Integer Dim BSlideAlongBeam As System.Integer   instance.SetManualEnd1ConnectionType(BHingeIstDir, BHinge2ndDir, BHingeAlongBeam, BSlide1stDir, BSlide2ndDir, BSlideAlongBeam) ``` | |

| C# |  |
| --- | --- |
| ``` void SetManualEnd1ConnectionType(     System.int BHingeIstDir,    System.int BHinge2ndDir,    System.int BHingeAlongBeam,    System.int BSlide1stDir,    System.int BSlide2ndDir,    System.int BSlideAlongBeam ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetManualEnd1ConnectionType(  &   System.int BHingeIstDir, &   System.int BHinge2ndDir, &   System.int BHingeAlongBeam, &   System.int BSlide1stDir, &   System.int BSlide2ndDir, &   System.int BSlideAlongBeam ) ``` | |

#### Parameters

*BHingeIstDir*
:   1 to set the moment about the first direction of the cross section to zero so that the end can rotate about this direction, 0 to not

*BHinge2ndDir*
:   1 to set the moment about the second direction of the cross section to zero so that the end can rotate about this direction, 0 to not

*BHingeAlongBeam*
:   1 to set the moment about the axial direction of the beam to zero so that the end can rotate about this direction, 0 to not

*BSlide1stDir*
:   1 to set the force in the first direction of the cross section to zero so that the end can translate along this direction, 0 to not

*BSlide2ndDir*
:   1 to set the force in the second direction of the cross section to zero so that the end can translate along this direction, 0 to not

*BSlideAlongBeam*
:   1 to set the force in the axial direction of the beam to zero so that the end can translate along this direction, 0 to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWBeamBody::SetManualEnd1ConnectionType.

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method, you must set [ICWBeamBody::BeamEnd1ConnectionType](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBeamBody~BeamEnd1ConnectionType.html) to swsBeamBodyConnectionManual.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWBeamBody Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody.html)

[ICWBeamBody Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody_members.html)

[ICWBeamBody::SetManualEnd2ConnectionType Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~SetManualEnd2ConnectionType.html)

[ICWBeamBody::BeamEnd2ConnectionType Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~BeamEnd2ConnectionType.html)

[ICWBeamBody::GetManualEnd1ConnectionType Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~GetManualEnd1ConnectionType.html)

[ICWBeamBody::GetManualEnd2ConnectionType Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~GetManualEnd2ConnectionType.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2010 SP0