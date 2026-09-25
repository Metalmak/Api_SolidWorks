<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMoveCopyBodyFeatureData~AddMate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddMate Method (IMoveCopyBodyFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IMoveCopyBodyFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMoveCopyBodyFeatureData.html) : AddMate Method (IMoveCopyBodyFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*MateEntVar*
:   Array of the entities to use to create a mate (see **Remarks**)

*MateTypeFromEnum*
:   Type of mate as defined in swMateType\_e

*AlignFromEnum*
:   Type of alignment as defined in swMateAlign\_e

*Distance*
:   Distance to use with distance or limit mates

*Angle*
:   Angle to use with angle mates

*ErrorStatus*
:   Success or error as defined by swAddMateError\_e

Adds a mate to the feature.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddMate( _    ByVal MateEntVar As System.Object, _    ByVal MateTypeFromEnum As System.Integer, _    ByVal AlignFromEnum As System.Integer, _    ByVal Distance As System.Double, _    ByVal Angle As System.Double, _    ByRef ErrorStatus As System.Integer _ ) As Mate2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IMoveCopyBodyFeatureData Dim MateEntVar As System.Object Dim MateTypeFromEnum As System.Integer Dim AlignFromEnum As System.Integer Dim Distance As System.Double Dim Angle As System.Double Dim ErrorStatus As System.Integer Dim value As Mate2   value = instance.AddMate(MateEntVar, MateTypeFromEnum, AlignFromEnum, Distance, Angle, ErrorStatus) ``` | |

| C# |  |
| --- | --- |
| ``` Mate2 AddMate(     System.object MateEntVar,    System.int MateTypeFromEnum,    System.int AlignFromEnum,    System.double Distance,    System.double Angle,    out System.int ErrorStatus ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Mate2^ AddMate(  &   System.Object^ MateEntVar, &   System.int MateTypeFromEnum, &   System.int AlignFromEnum, &   System.double Distance, &   System.double Angle, &   [Out] System.int ErrorStatus ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*MateEntVar*
:   Array of the entities to use to create a mate (see **Remarks**)

*MateTypeFromEnum*
:   Type of mate as defined in swMateType\_e

*AlignFromEnum*
:   Type of alignment as defined in swMateAlign\_e

*Distance*
:   Distance to use with distance or limit mates

*Angle*
:   Angle to use with angle mates

*ErrorStatus*
:   Success or error as defined by swAddMateError\_e

#### Return Value

[Mate](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMate2.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See MoveCopyBodyFeatureData::AddMate.

# ![](dotnetimages/collapse.gif)Remarks

You can specify MateEntVar with either an array of mate entities or null. If you specify null, then before calling this method, you must call [IModelDocExtension::SelectByID2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByID2.html) with a selection mark of 1 to select each mate entity.

See Accessing Selections that Define Features for additional details on using this method.

# ![](dotnetimages/collapse.gif)See Also

####

[IMoveCopyBodyFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMoveCopyBodyFeatureData.html)

[IMoveCopyBodyFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMoveCopyBodyFeatureData_members.html)

[IMoveCopyBodyFeatureData::IAddMate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMoveCopyBodyFeatureData~IAddMate.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2006 FCS, Revision Number 14.0