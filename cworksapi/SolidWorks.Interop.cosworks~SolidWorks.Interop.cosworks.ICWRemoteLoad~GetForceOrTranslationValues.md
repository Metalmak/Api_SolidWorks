<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~GetForceOrTranslationValues.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetForceOrTranslationValues Method (ICWRemoteLoad) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html) : GetForceOrTranslationValues Method (ICWRemoteLoad) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BInclude*
:   1 to get force or translation values, 0 to not (see **Remarks**)

*BXValue*
:   1 to get the value in the x direction, 0 to not

*DXValue*
:   Force or translation in the x direction; valid only if BXValue = 1

*BYValue*
:   1 to get the value in the y direction; 0 to not

*DYValue*
:   Force or translation in the y direction; valid only if BYValue = 1

*BZValue*
:   1 to get the value in the z direction; 0 to not

*DZValue*
:   Force or translation in the z direction; valid only if BZValue = 1

Obsolete. Superseded by [ICWRemoteLoad::GetForceOrTranslationValues2](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRadiation~UseTimeCurve2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetForceOrTranslationValues( _    ByRef BInclude As System.Integer, _    ByRef BXValue As System.Integer, _    ByRef DXValue As System.Double, _    ByRef BYValue As System.Integer, _    ByRef DYValue As System.Double, _    ByRef BZValue As System.Integer, _    ByRef DZValue As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRemoteLoad Dim BInclude As System.Integer Dim BXValue As System.Integer Dim DXValue As System.Double Dim BYValue As System.Integer Dim DYValue As System.Double Dim BZValue As System.Integer Dim DZValue As System.Double   instance.GetForceOrTranslationValues(BInclude, BXValue, DXValue, BYValue, DYValue, BZValue, DZValue) ``` | |

| C# |  |
| --- | --- |
| ``` void GetForceOrTranslationValues(     out System.int BInclude,    out System.int BXValue,    out System.double DXValue,    out System.int BYValue,    out System.double DYValue,    out System.int BZValue,    out System.double DZValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetForceOrTranslationValues(  &   [Out] System.int BInclude, &   [Out] System.int BXValue, &   [Out] System.double DXValue, &   [Out] System.int BYValue, &   [Out] System.double DYValue, &   [Out] System.int BZValue, &   [Out] System.double DZValue ) ``` | |

#### Parameters

*BInclude*
:   1 to get force or translation values, 0 to not (see **Remarks**)

*BXValue*
:   1 to get the value in the x direction, 0 to not

*DXValue*
:   Force or translation in the x direction; valid only if BXValue = 1

*BYValue*
:   1 to get the value in the y direction; 0 to not

*DYValue*
:   Force or translation in the y direction; valid only if BYValue = 1

*BZValue*
:   1 to get the value in the z direction; 0 to not

*DZValue*
:   Force or translation in the z direction; valid only if BZValue = 1

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWRemoteLoad::GetForceOrTranslationValues.

# ![](dotnetimages/collapse.gif)Remarks

| This method gets components of ... | If [ICWRemoteLoad::LoadType](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWRemoteLoad~LoadType.html) is ... |
| --- | --- |
| Force | swsRemoteLoadType\_e.swsRemoteLoadType\_DirectLoad  - or -  swsRemoteLoadType\_e.swsRemoteLoadType\_RigidLoadOrMass |
| Translation | swsRemoteLoadType\_e.swsRemoteLoadType\_DirectDisplacement  - or -  swsRemoteLoadType\_e.swsRemoteLoadType\_RigidDisplacement |

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html)

[ICWRemoteLoad Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad_members.html)

[ICWRemoteLoad::SetForceOrTranslationValues Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~SetForceOrTranslationValues.html)

[ICWRemoteLoad::ForceOrTranslationUnit Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~ForceOrTranslationUnit.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0