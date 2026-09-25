<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~EditMate3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| EditMate3 Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : EditMate3 Method (IAssemblyDoc) |

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
:   Type of alignment as defined in swMateAlign\_e

*Flip*
:   True to flip the component, false to not

*Distance*
:   Distance value; valid only if MateTypeFromEnum is swMateType\_e.swMateDISTANCE

*DistanceAbsUpperLimit*
:   Absolute maximum distance allowed; valid only if MateTypeFromEnum is swMateType\_e.swMateDISTANCE

*DistanceAbsLowerLimit*
:   Absolute minimum distance allowed; valid only if MateTypeFromEnum is swMateType\_e.swMateDISTANCE

*GearRatioNumerator*
:   Gear ratio numerator value; valid only if MateTypeFromEnum is swMateType\_e.swMateGEAR

*GearRatioDenominator*
:   Gear ratio denominator value; valid only if MateTypeFromEnum is swMateType\_e.swMateGEAR

*Angle*
:   Angle value; valid only if MateTypeFromEnum is swMateType\_e.swMateANGLE

*AngleAbsUpperLimit*
:   Absolute maximum angle allowed; valid only if MateTypeFromEnum is swMateType\_e.swMateANGLE

*AngleAbsLowerLimit*
:   Absolute minimum angle allowed; valid only if MateTypeFromEnum is swMateType\_e.swMateANGLE

*ForPositioningOnly*
:   True to only position the components according to the mating relationship and not return a mate, false to return a mate

*LockRotation*
:   True to lock component rotation, false to not

*WidthMateOption*
:   Width mate options as defined in swMateWidthOptions\_e; valid only if MateTypeFromEnum is swMateType\_e.swMateWIDTH

*ErrorStatus*
:   Success or error as defined by swAddMateError\_e

Obsolete. Superseded by [IAssemblyDoc::EditMate4](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~EditMate4.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub EditMate3( _    ByVal MateTypeFromEnum As System.Integer, _    ByVal AlignFromEnum As System.Integer, _    ByVal Flip As System.Boolean, _    ByVal Distance As System.Double, _    ByVal DistanceAbsUpperLimit As System.Double, _    ByVal DistanceAbsLowerLimit As System.Double, _    ByVal GearRatioNumerator As System.Double, _    ByVal GearRatioDenominator As System.Double, _    ByVal Angle As System.Double, _    ByVal AngleAbsUpperLimit As System.Double, _    ByVal AngleAbsLowerLimit As System.Double, _    ByVal ForPositioningOnly As System.Boolean, _    ByVal LockRotation As System.Boolean, _    ByVal WidthMateOption As System.Integer, _    ByRef ErrorStatus As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim MateTypeFromEnum As System.Integer Dim AlignFromEnum As System.Integer Dim Flip As System.Boolean Dim Distance As System.Double Dim DistanceAbsUpperLimit As System.Double Dim DistanceAbsLowerLimit As System.Double Dim GearRatioNumerator As System.Double Dim GearRatioDenominator As System.Double Dim Angle As System.Double Dim AngleAbsUpperLimit As System.Double Dim AngleAbsLowerLimit As System.Double Dim ForPositioningOnly As System.Boolean Dim LockRotation As System.Boolean Dim WidthMateOption As System.Integer Dim ErrorStatus As System.Integer   instance.EditMate3(MateTypeFromEnum, AlignFromEnum, Flip, Distance, DistanceAbsUpperLimit, DistanceAbsLowerLimit, GearRatioNumerator, GearRatioDenominator, Angle, AngleAbsUpperLimit, AngleAbsLowerLimit, ForPositioningOnly, LockRotation, WidthMateOption, ErrorStatus) ``` | |

| C# |  |
| --- | --- |
| ``` void EditMate3(     System.int MateTypeFromEnum,    System.int AlignFromEnum,    System.bool Flip,    System.double Distance,    System.double DistanceAbsUpperLimit,    System.double DistanceAbsLowerLimit,    System.double GearRatioNumerator,    System.double GearRatioDenominator,    System.double Angle,    System.double AngleAbsUpperLimit,    System.double AngleAbsLowerLimit,    System.bool ForPositioningOnly,    System.bool LockRotation,    System.int WidthMateOption,    out System.int ErrorStatus ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void EditMate3(  &   System.int MateTypeFromEnum, &   System.int AlignFromEnum, &   System.bool Flip, &   System.double Distance, &   System.double DistanceAbsUpperLimit, &   System.double DistanceAbsLowerLimit, &   System.double GearRatioNumerator, &   System.double GearRatioDenominator, &   System.double Angle, &   System.double AngleAbsUpperLimit, &   System.double AngleAbsLowerLimit, &   System.bool ForPositioningOnly, &   System.bool LockRotation, &   System.int WidthMateOption, &   [Out] System.int ErrorStatus ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*MateTypeFromEnum*
:   Type of mate as defined in swMateType\_e

*AlignFromEnum*
:   Type of alignment as defined in swMateAlign\_e

*Flip*
:   True to flip the component, false to not

*Distance*
:   Distance value; valid only if MateTypeFromEnum is swMateType\_e.swMateDISTANCE

*DistanceAbsUpperLimit*
:   Absolute maximum distance allowed; valid only if MateTypeFromEnum is swMateType\_e.swMateDISTANCE

*DistanceAbsLowerLimit*
:   Absolute minimum distance allowed; valid only if MateTypeFromEnum is swMateType\_e.swMateDISTANCE

*GearRatioNumerator*
:   Gear ratio numerator value; valid only if MateTypeFromEnum is swMateType\_e.swMateGEAR

*GearRatioDenominator*
:   Gear ratio denominator value; valid only if MateTypeFromEnum is swMateType\_e.swMateGEAR

*Angle*
:   Angle value; valid only if MateTypeFromEnum is swMateType\_e.swMateANGLE

*AngleAbsUpperLimit*
:   Absolute maximum angle allowed; valid only if MateTypeFromEnum is swMateType\_e.swMateANGLE

*AngleAbsLowerLimit*
:   Absolute minimum angle allowed; valid only if MateTypeFromEnum is swMateType\_e.swMateANGLE

*ForPositioningOnly*
:   True to only position the components according to the mating relationship and not return a mate, false to return a mate

*LockRotation*
:   True to lock component rotation, false to not

*WidthMateOption*
:   Width mate options as defined in swMateWidthOptions\_e; valid only if MateTypeFromEnum is swMateType\_e.swMateWIDTH

*ErrorStatus*
:   Success or error as defined by swAddMateError\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::EditMate3.

# ![](dotnetimages/collapse.gif)Example

[Edit Mate (VBA)](Edit_Mate_Example_VB.htm)

[Edit Mate (VB.NET)](Edit_Mate_Example_VBNET.htm)

[Edit Mate (C#)](Edit_Mate_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

The first selections should be the two items that are mated (that is, two faces, edge and face, and so on), and the third selection should be the mate feature to be edited. The mate feature must be selected last. The two mated items must be selected with a selection mark of 1. See [ISelectData](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISelectData.html) or [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) for details on using selection marks.

If MateTypeFromEnum is swMateType\_e.swMateDISTANCE or swMateType\_e.swMateANGLE, and the mate is applied to the closest position that meets the mate condition specified by Distance or Angle, then setting Flip to true moves the assembly to the other possible mate position.

This method does not support editing **Inplace** mates.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IAssemblyDoc::AddMate5](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddMate5.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0