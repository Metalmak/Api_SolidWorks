<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~EditMate2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EditMate2 Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : EditMate2 Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*MateTypeFromEnum*
:   Type of mate as defined in swMateType\_e

*AlignFromEnum*
:   Type of alignment desired as defined in swMateAlign\_e

*Flip*
:   True to flip the component, false to not

*Distance*
:   Distance value to use with distance or limit mates

*DistanceAbsUpperLimit*
:   Absolute maximum distance allowed

*DistanceAbsLowerLimit*
:   Absolute minimum distance allowed

*GearRatioNumerator*
:   Gear ratio numerator value for gear mates

*GearRatioDenominator*
:   Gear ratio denominator value for gear mates

*Angle*
:   Angle value to use with angle mates

*AngleAbsUpperLimit*
:   Absolute maximum angle allowed

*AngleAbsLowerLimit*
:   Absolute minimum angle allowed

*ErrorStatus*
:   Success or error as defined by swAddMateError\_e

Obsolete. Superseded by [IAssemblyDoc::EditMate3.](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAssemblyDoc~EditMate3.html)

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub EditMate2( _    ByVal MateTypeFromEnum As System.Integer, _    ByVal AlignFromEnum As System.Integer, _    ByVal Flip As System.Boolean, _    ByVal Distance As System.Double, _    ByVal DistanceAbsUpperLimit As System.Double, _    ByVal DistanceAbsLowerLimit As System.Double, _    ByVal GearRatioNumerator As System.Double, _    ByVal GearRatioDenominator As System.Double, _    ByVal Angle As System.Double, _    ByVal AngleAbsUpperLimit As System.Double, _    ByVal AngleAbsLowerLimit As System.Double, _    ByRef ErrorStatus As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim MateTypeFromEnum As System.Integer Dim AlignFromEnum As System.Integer Dim Flip As System.Boolean Dim Distance As System.Double Dim DistanceAbsUpperLimit As System.Double Dim DistanceAbsLowerLimit As System.Double Dim GearRatioNumerator As System.Double Dim GearRatioDenominator As System.Double Dim Angle As System.Double Dim AngleAbsUpperLimit As System.Double Dim AngleAbsLowerLimit As System.Double Dim ErrorStatus As System.Integer   instance.EditMate2(MateTypeFromEnum, AlignFromEnum, Flip, Distance, DistanceAbsUpperLimit, DistanceAbsLowerLimit, GearRatioNumerator, GearRatioDenominator, Angle, AngleAbsUpperLimit, AngleAbsLowerLimit, ErrorStatus) ``` | |

| C# |  |
| --- | --- |
| ``` void EditMate2(     System.int MateTypeFromEnum,    System.int AlignFromEnum,    System.bool Flip,    System.double Distance,    System.double DistanceAbsUpperLimit,    System.double DistanceAbsLowerLimit,    System.double GearRatioNumerator,    System.double GearRatioDenominator,    System.double Angle,    System.double AngleAbsUpperLimit,    System.double AngleAbsLowerLimit,    out System.int ErrorStatus ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void EditMate2(  &   System.int MateTypeFromEnum, &   System.int AlignFromEnum, &   System.bool Flip, &   System.double Distance, &   System.double DistanceAbsUpperLimit, &   System.double DistanceAbsLowerLimit, &   System.double GearRatioNumerator, &   System.double GearRatioDenominator, &   System.double Angle, &   System.double AngleAbsUpperLimit, &   System.double AngleAbsLowerLimit, &   [Out] System.int ErrorStatus ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*MateTypeFromEnum*
:   Type of mate as defined in swMateType\_e

*AlignFromEnum*
:   Type of alignment desired as defined in swMateAlign\_e

*Flip*
:   True to flip the component, false to not

*Distance*
:   Distance value to use with distance or limit mates

*DistanceAbsUpperLimit*
:   Absolute maximum distance allowed

*DistanceAbsLowerLimit*
:   Absolute minimum distance allowed

*GearRatioNumerator*
:   Gear ratio numerator value for gear mates

*GearRatioDenominator*
:   Gear ratio denominator value for gear mates

*Angle*
:   Angle value to use with angle mates

*AngleAbsUpperLimit*
:   Absolute maximum angle allowed

*AngleAbsLowerLimit*
:   Absolute minimum angle allowed

*ErrorStatus*
:   Success or error as defined by swAddMateError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::EditMate2.

# ![](dotnetimages/collapse.gif)Remarks

The first selection should be the two items that are mated (that is, two faces, edge and face, and so on), and the third selection should be the mate feature to be edited. The mate feature must be selected last. The two mated items must be selected with a selection mark of 1. See [ISelectData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectData.html) or [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) for details on using selection marks.

If mateType is swMateDISTANCE or swMateANGLE when the mate is applied to the closest position that meets the mate condition specified by distance or angle, then setting flip to True moves the assembly to the other possible mate position.

This method does not support editing **Inplace** mates.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IAssemblyDoc::AddMate3 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddMate3.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2004 FCS, Revision Number 12