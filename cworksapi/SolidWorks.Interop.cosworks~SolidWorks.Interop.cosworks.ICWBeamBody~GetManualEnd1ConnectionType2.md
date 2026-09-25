<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~GetManualEnd1ConnectionType2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetManualEnd1ConnectionType2 Method (ICWBeamBody) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWBeamBody Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody.html) : GetManualEnd1ConnectionType2 Method (ICWBeamBody) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BHingeIstDir*
:   -1 or true if the moment about the first direction of the cross section is known to be zero so that the end can rotate about this direction, 0 or false if not

*BHinge2ndDir*
:   -1 or true if the moment about the second direction of the cross section is known to be zero so that the end can rotate about this direction, 0 or false if not

*BHingeAlongBeam*
:   -1 or true if the moment about the axial direction of the beam is known to be zero so that the end can rotate about this direction, 0 or false if not

*BSlide1stDir*
:   -1 or true if the force in the first direction of the cross section is known to be zero so that the end can translate along this direction, 0 or false if not

*BSlide2ndDir*
:   -1 or true if the force in the second direction of the cross section is known to be zero so that the end can translate along this direction, 0 or false if not

*BSlideAlongBeam*
:   -1 or true if the force in the axial direction of the beam is known to be zero so that the end can translate along this direction, 0 or false if not

Gets whether manual forces and moments are known to be zero for the End1 connection of the beam.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetManualEnd1ConnectionType2( _    ByRef BHingeIstDir As System.Boolean, _    ByRef BHinge2ndDir As System.Boolean, _    ByRef BHingeAlongBeam As System.Boolean, _    ByRef BSlide1stDir As System.Boolean, _    ByRef BSlide2ndDir As System.Boolean, _    ByRef BSlideAlongBeam As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWBeamBody Dim BHingeIstDir As System.Boolean Dim BHinge2ndDir As System.Boolean Dim BHingeAlongBeam As System.Boolean Dim BSlide1stDir As System.Boolean Dim BSlide2ndDir As System.Boolean Dim BSlideAlongBeam As System.Boolean   instance.GetManualEnd1ConnectionType2(BHingeIstDir, BHinge2ndDir, BHingeAlongBeam, BSlide1stDir, BSlide2ndDir, BSlideAlongBeam) ``` | |

| C# |  |
| --- | --- |
| ``` void GetManualEnd1ConnectionType2(     out System.bool BHingeIstDir,    out System.bool BHinge2ndDir,    out System.bool BHingeAlongBeam,    out System.bool BSlide1stDir,    out System.bool BSlide2ndDir,    out System.bool BSlideAlongBeam ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetManualEnd1ConnectionType2(  &   [Out] System.bool BHingeIstDir, &   [Out] System.bool BHinge2ndDir, &   [Out] System.bool BHingeAlongBeam, &   [Out] System.bool BSlide1stDir, &   [Out] System.bool BSlide2ndDir, &   [Out] System.bool BSlideAlongBeam ) ``` | |

#### Parameters

*BHingeIstDir*
:   -1 or true if the moment about the first direction of the cross section is known to be zero so that the end can rotate about this direction, 0 or false if not

*BHinge2ndDir*
:   -1 or true if the moment about the second direction of the cross section is known to be zero so that the end can rotate about this direction, 0 or false if not

*BHingeAlongBeam*
:   -1 or true if the moment about the axial direction of the beam is known to be zero so that the end can rotate about this direction, 0 or false if not

*BSlide1stDir*
:   -1 or true if the force in the first direction of the cross section is known to be zero so that the end can translate along this direction, 0 or false if not

*BSlide2ndDir*
:   -1 or true if the force in the second direction of the cross section is known to be zero so that the end can translate along this direction, 0 or false if not

*BSlideAlongBeam*
:   -1 or true if the force in the axial direction of the beam is known to be zero so that the end can translate along this direction, 0 or false if not

# ![](dotnetimages/collapse.gif)Remarks

This method returns booleans or integers in the out parameters, depending on their prior declarations.

If out parameters are cast as:

* Booleans, true or false is returned in each out parameter.* Longs or integers, -1 (=true) or 0 (=false) is returned in each out parameter.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWBeamBody Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody.html)

[ICWBeamBody Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30