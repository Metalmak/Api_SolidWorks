<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad~GetForceOrTranslationValues2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetForceOrTranslationValues2 Method (ICWRemoteLoad) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html) : GetForceOrTranslationValues2 Method (ICWRemoteLoad) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*BInclude*
:   -1 or true to get force or translation values, 0 or false to not (see **Remarks**)

*BXValue*
:   -1 or true to get the value in the x direction, 0 or false to not

*DXValue*
:   Force or translation in the x direction; valid only if BXValue = -1

*BYValue*
:   -1 or true to get the value in the y direction; 0 or false to not

*DYValue*
:   Force or translation in the y direction; valid only if BYValue = -1

*BZValue*
:   -1 or true to get the value in the z direction; 0 or false to not

*DZValue*
:   Force or translation in the z direction; valid only if BZValue = -1

Gets the components of force or translation for this remote load.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetForceOrTranslationValues2( _    ByRef BInclude As System.Boolean, _    ByRef BXValue As System.Boolean, _    ByRef DXValue As System.Double, _    ByRef BYValue As System.Boolean, _    ByRef DYValue As System.Double, _    ByRef BZValue As System.Boolean, _    ByRef DZValue As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWRemoteLoad Dim BInclude As System.Boolean Dim BXValue As System.Boolean Dim DXValue As System.Double Dim BYValue As System.Boolean Dim DYValue As System.Double Dim BZValue As System.Boolean Dim DZValue As System.Double   instance.GetForceOrTranslationValues2(BInclude, BXValue, DXValue, BYValue, DYValue, BZValue, DZValue) ``` | |

| C# |  |
| --- | --- |
| ``` void GetForceOrTranslationValues2(     out System.bool BInclude,    out System.bool BXValue,    out System.double DXValue,    out System.bool BYValue,    out System.double DYValue,    out System.bool BZValue,    out System.double DZValue ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetForceOrTranslationValues2(  &   [Out] System.bool BInclude, &   [Out] System.bool BXValue, &   [Out] System.double DXValue, &   [Out] System.bool BYValue, &   [Out] System.double DYValue, &   [Out] System.bool BZValue, &   [Out] System.double DZValue ) ``` | |

#### Parameters

*BInclude*
:   -1 or true to get force or translation values, 0 or false to not (see **Remarks**)

*BXValue*
:   -1 or true to get the value in the x direction, 0 or false to not

*DXValue*
:   Force or translation in the x direction; valid only if BXValue = -1

*BYValue*
:   -1 or true to get the value in the y direction; 0 or false to not

*DYValue*
:   Force or translation in the y direction; valid only if BYValue = -1

*BZValue*
:   -1 or true to get the value in the z direction; 0 or false to not

*DZValue*
:   Force or translation in the z direction; valid only if BZValue = -1

# ![](dotnetimages/collapse.gif)Example

See the [ICWRemoteLoad](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

This method returns booleans or integers in the out parameters, depending on their prior declarations.

If out parameters are cast as:

* Booleans, true or false is returned in each out parameter.* Longs or integers, -1 (=true) or 0 (=false) is returned in each out parameter.

| This method gets components of ... | If [ICWRemoteLoad::LoadType](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWRemoteLoad~LoadType.html) is ... |
| --- | --- |
| Force | swsRemoteLoadType\_e.swsRemoteLoadType\_DirectLoad  - or -  swsRemoteLoadType\_e.swsRemoteLoadType\_RigidLoadOrMass |
| Translation | swsRemoteLoadType\_e.swsRemoteLoadType\_DirectDisplacement  - or -  swsRemoteLoadType\_e.swsRemoteLoadType\_RigidDisplacement |

# ![](dotnetimages/collapse.gif)See Also

####

[ICWRemoteLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad.html)

[ICWRemoteLoad Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWRemoteLoad_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30