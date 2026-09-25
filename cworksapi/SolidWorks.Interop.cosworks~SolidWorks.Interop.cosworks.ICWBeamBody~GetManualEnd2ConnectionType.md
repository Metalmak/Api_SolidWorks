<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~GetManualEnd2ConnectionType.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetManualEnd2ConnectionType Method (ICWBeamBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWBeamBody Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody.html) : GetManualEnd2ConnectionType Method (ICWBeamBody) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BHingeIstDir*
:   1 if the moment about the first direction of the cross section is known to be zero so that the end can rotate about this direction, 0 if not

*BHinge2ndDir*
:   1 if the moment about the second direction of the cross section is known to be zero so that the end can rotate about this direction, 0 if not

*BHingeAlongBeam*
:   1 if the moment about the axial direction of the beam is known to be zero so that the end can rotate about this direction, 0 if not

*BSlide1stDir*
:   1 if the force in the first direction of the cross section is known to be zero so that the end can translate along this direction, 0 if not

*BSlide2ndDir*
:   1 if the force in the second direction of the cross section is known to be zero so that the end can translate along this direction, 0 if not

*BSlideAlongBeam*
:   1 if the force in the axial direction of the beam is known to be zero so that the end can translate along this direction, 0 if not

Obsolete. Superseded by [ICWBeamBody::GetManualEnd2ConnectionType2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~GetManualEnd2ConnectionType2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetManualEnd2ConnectionType( _    ByRef BHingeIstDir As System.Integer, _    ByRef BHinge2ndDir As System.Integer, _    ByRef BHingeAlongBeam As System.Integer, _    ByRef BSlide1stDir As System.Integer, _    ByRef BSlide2ndDir As System.Integer, _    ByRef BSlideAlongBeam As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWBeamBody Dim BHingeIstDir As System.Integer Dim BHinge2ndDir As System.Integer Dim BHingeAlongBeam As System.Integer Dim BSlide1stDir As System.Integer Dim BSlide2ndDir As System.Integer Dim BSlideAlongBeam As System.Integer   instance.GetManualEnd2ConnectionType(BHingeIstDir, BHinge2ndDir, BHingeAlongBeam, BSlide1stDir, BSlide2ndDir, BSlideAlongBeam) ``` | |

| C# |  |
| --- | --- |
| ``` void GetManualEnd2ConnectionType(     out System.int BHingeIstDir,    out System.int BHinge2ndDir,    out System.int BHingeAlongBeam,    out System.int BSlide1stDir,    out System.int BSlide2ndDir,    out System.int BSlideAlongBeam ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetManualEnd2ConnectionType(  &   [Out] System.int BHingeIstDir, &   [Out] System.int BHinge2ndDir, &   [Out] System.int BHingeAlongBeam, &   [Out] System.int BSlide1stDir, &   [Out] System.int BSlide2ndDir, &   [Out] System.int BSlideAlongBeam ) ``` | |

#### Parameters

*BHingeIstDir*
:   1 if the moment about the first direction of the cross section is known to be zero so that the end can rotate about this direction, 0 if not

*BHinge2ndDir*
:   1 if the moment about the second direction of the cross section is known to be zero so that the end can rotate about this direction, 0 if not

*BHingeAlongBeam*
:   1 if the moment about the axial direction of the beam is known to be zero so that the end can rotate about this direction, 0 if not

*BSlide1stDir*
:   1 if the force in the first direction of the cross section is known to be zero so that the end can translate along this direction, 0 if not

*BSlide2ndDir*
:   1 if the force in the second direction of the cross section is known to be zero so that the end can translate along this direction, 0 if not

*BSlideAlongBeam*
:   1 if the force in the axial direction of the beam is known to be zero so that the end can translate along this direction, 0 if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWBeamBody::GeManualEnd2ConnectionType.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWBeamBody Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody.html)

[ICWBeamBody Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2010