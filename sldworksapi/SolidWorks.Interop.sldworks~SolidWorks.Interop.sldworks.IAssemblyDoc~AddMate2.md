<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddMate2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddMate2 Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : AddMate2 Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*MateTypeFromEnum*

*AlignFromEnum*

*Flip*

*Distance*

*DistanceAbsUpperLimit*

*DistanceAbsLowerLimit*

*GearRatioNumerator*

*GearRatioDenominator*

*Angle*

*AngleAbsUpperLimit*

*AngleAbsLowerLimit*

*ErrorStatus*

Obsolete. Superseded by [IAssemblyDoc::AddMate3](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IAssemblyDoc~AddMate3.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddMate2( _    ByVal MateTypeFromEnum As System.Integer, _    ByVal AlignFromEnum As System.Integer, _    ByVal Flip As System.Boolean, _    ByVal Distance As System.Double, _    ByVal DistanceAbsUpperLimit As System.Double, _    ByVal DistanceAbsLowerLimit As System.Double, _    ByVal GearRatioNumerator As System.Double, _    ByVal GearRatioDenominator As System.Double, _    ByVal Angle As System.Double, _    ByVal AngleAbsUpperLimit As System.Double, _    ByVal AngleAbsLowerLimit As System.Double, _    ByRef ErrorStatus As System.Integer _ ) As Mate2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim MateTypeFromEnum As System.Integer Dim AlignFromEnum As System.Integer Dim Flip As System.Boolean Dim Distance As System.Double Dim DistanceAbsUpperLimit As System.Double Dim DistanceAbsLowerLimit As System.Double Dim GearRatioNumerator As System.Double Dim GearRatioDenominator As System.Double Dim Angle As System.Double Dim AngleAbsUpperLimit As System.Double Dim AngleAbsLowerLimit As System.Double Dim ErrorStatus As System.Integer Dim value As Mate2   value = instance.AddMate2(MateTypeFromEnum, AlignFromEnum, Flip, Distance, DistanceAbsUpperLimit, DistanceAbsLowerLimit, GearRatioNumerator, GearRatioDenominator, Angle, AngleAbsUpperLimit, AngleAbsLowerLimit, ErrorStatus) ``` | |

| C# |  |
| --- | --- |
| ``` Mate2 AddMate2(     System.int MateTypeFromEnum,    System.int AlignFromEnum,    System.bool Flip,    System.double Distance,    System.double DistanceAbsUpperLimit,    System.double DistanceAbsLowerLimit,    System.double GearRatioNumerator,    System.double GearRatioDenominator,    System.double Angle,    System.double AngleAbsUpperLimit,    System.double AngleAbsLowerLimit,    out System.int ErrorStatus ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Mate2^ AddMate2(  &   System.int MateTypeFromEnum, &   System.int AlignFromEnum, &   System.bool Flip, &   System.double Distance, &   System.double DistanceAbsUpperLimit, &   System.double DistanceAbsLowerLimit, &   System.double GearRatioNumerator, &   System.double GearRatioDenominator, &   System.double Angle, &   System.double AngleAbsUpperLimit, &   System.double AngleAbsLowerLimit, &   [Out] System.int ErrorStatus ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*MateTypeFromEnum*

*AlignFromEnum*

*Flip*

*Distance*

*DistanceAbsUpperLimit*

*DistanceAbsLowerLimit*

*GearRatioNumerator*

*GearRatioDenominator*

*Angle*

*AngleAbsUpperLimit*

*AngleAbsLowerLimit*

*ErrorStatus*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::AddMate2.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)