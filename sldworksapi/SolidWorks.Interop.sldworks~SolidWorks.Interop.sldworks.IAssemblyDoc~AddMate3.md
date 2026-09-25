<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddMate3.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddMate3 Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : AddMate3 Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*MateTypeFromEnum*
:   Type of mate as defined in swMateType\_e (see **Remarks**)

*AlignFromEnum*
:   Type of alignment as defined in swMateAlign\_e

*Flip*
:   True to flip the component, false otherwise

*Distance*
:   Distance value to use with distance or limit mates

*DistanceAbsUpperLimit*
:   Absolute maximum distance value (see **Remarks**)

*DistanceAbsLowerLimit*
:   Absolute minimum distance value  (see Remarks)

*GearRatioNumerator*
:   Gear ratio numerator value for gear mates

*GearRatioDenominator*
:   Gear ratio denominator value for gear mates

*Angle*
:   Angle value to use with angle mates

*AngleAbsUpperLimit*
:   Absolute maximum angle value

*AngleAbsLowerLimit*
:   Absolute maximum angle value

*ForPositioningOnly*
:   True to only position the components according to the mating relationship and not create and return a mate, false to not

*ErrorStatus*
:   Success or error as defined by swAddMateError\_e

Obsolete. Superseded by [IAssemblyDoc::AddMate4](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAssemblyDoc~AddMate4.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddMate3( _    ByVal MateTypeFromEnum As System.Integer, _    ByVal AlignFromEnum As System.Integer, _    ByVal Flip As System.Boolean, _    ByVal Distance As System.Double, _    ByVal DistanceAbsUpperLimit As System.Double, _    ByVal DistanceAbsLowerLimit As System.Double, _    ByVal GearRatioNumerator As System.Double, _    ByVal GearRatioDenominator As System.Double, _    ByVal Angle As System.Double, _    ByVal AngleAbsUpperLimit As System.Double, _    ByVal AngleAbsLowerLimit As System.Double, _    ByVal ForPositioningOnly As System.Boolean, _    ByRef ErrorStatus As System.Integer _ ) As Mate2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim MateTypeFromEnum As System.Integer Dim AlignFromEnum As System.Integer Dim Flip As System.Boolean Dim Distance As System.Double Dim DistanceAbsUpperLimit As System.Double Dim DistanceAbsLowerLimit As System.Double Dim GearRatioNumerator As System.Double Dim GearRatioDenominator As System.Double Dim Angle As System.Double Dim AngleAbsUpperLimit As System.Double Dim AngleAbsLowerLimit As System.Double Dim ForPositioningOnly As System.Boolean Dim ErrorStatus As System.Integer Dim value As Mate2   value = instance.AddMate3(MateTypeFromEnum, AlignFromEnum, Flip, Distance, DistanceAbsUpperLimit, DistanceAbsLowerLimit, GearRatioNumerator, GearRatioDenominator, Angle, AngleAbsUpperLimit, AngleAbsLowerLimit, ForPositioningOnly, ErrorStatus) ``` | |

| C# |  |
| --- | --- |
| ``` Mate2 AddMate3(     System.int MateTypeFromEnum,    System.int AlignFromEnum,    System.bool Flip,    System.double Distance,    System.double DistanceAbsUpperLimit,    System.double DistanceAbsLowerLimit,    System.double GearRatioNumerator,    System.double GearRatioDenominator,    System.double Angle,    System.double AngleAbsUpperLimit,    System.double AngleAbsLowerLimit,    System.bool ForPositioningOnly,    out System.int ErrorStatus ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Mate2^ AddMate3(  &   System.int MateTypeFromEnum, &   System.int AlignFromEnum, &   System.bool Flip, &   System.double Distance, &   System.double DistanceAbsUpperLimit, &   System.double DistanceAbsLowerLimit, &   System.double GearRatioNumerator, &   System.double GearRatioDenominator, &   System.double Angle, &   System.double AngleAbsUpperLimit, &   System.double AngleAbsLowerLimit, &   System.bool ForPositioningOnly, &   [Out] System.int ErrorStatus ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*MateTypeFromEnum*
:   Type of mate as defined in swMateType\_e (see **Remarks**)

*AlignFromEnum*
:   Type of alignment as defined in swMateAlign\_e

*Flip*
:   True to flip the component, false otherwise

*Distance*
:   Distance value to use with distance or limit mates

*DistanceAbsUpperLimit*
:   Absolute maximum distance value (see **Remarks**)

*DistanceAbsLowerLimit*
:   Absolute minimum distance value  (see Remarks)

*GearRatioNumerator*
:   Gear ratio numerator value for gear mates

*GearRatioDenominator*
:   Gear ratio denominator value for gear mates

*Angle*
:   Angle value to use with angle mates

*AngleAbsUpperLimit*
:   Absolute maximum angle value

*AngleAbsLowerLimit*
:   Absolute maximum angle value

*ForPositioningOnly*
:   True to only position the components according to the mating relationship and not create and return a mate, false to not

*ErrorStatus*
:   Success or error as defined by swAddMateError\_e

#### Return Value

[IMate2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMate2.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::AddMate3.

# ![](dotnetimages/collapse.gif)Remarks

To specify a distance mate without limits, set the DistanceAbsUpperLimit and DistanceAbsLowerLimit arguments equal to the distance argument's value.

If MateTypeFromEnum is swMateDISTANCE or swMateANGLE when the mate is applied to the closest position that meets the mate condition specified by distance or angle, then setting Flip to true moves the assembly to the other possible mate position.

To add a mate:

1. Call [IModelDoc2::ClearSelection2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~ClearSelection2.html) before selecting entities to mate.

   - Call [IModelDocExtension::SelectByID2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDocExtension~SelectByID2.html) to select entities to mate.

     If MateTypeFromEnum is swMateCAMFOLLOWER, then use a selection mark of 8 for the cam-follower face.

     If MateTypeFromEnum is swMateWIDTH and uses tab selections, then use a selection mark of 16. If MateTypeFromEnum is anything else, then use a selection mark of 1.

     - Call this method.

       - Call IModelDoc2::ClearSelection2 after the mate is created.

If nothing is preselected, then ErrorStatus is swAddMateError\_IncorrectSelections, and nothing is returned.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IAssemblyDoc::EditMate2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~EditMate2.html)

[IAssemblyDoc::CopyWithMates Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~CopyWithMates.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2005 SP2, Revision Number 13