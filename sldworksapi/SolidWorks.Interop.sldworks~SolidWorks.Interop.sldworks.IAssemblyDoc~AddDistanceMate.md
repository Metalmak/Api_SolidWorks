<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddDistanceMate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddDistanceMate Method (IAssemblyDoc) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html) : AddDistanceMate Method (IAssemblyDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*AlignFromEnum*
:   Type of alignment as defined in swMateAlign\_e

*Flip*
:   True to flip mate entities, false to not (see **Remarks**)

*Distance*
:   Distance value (see **Remarks**)

*DistanceAbsUpperLimit*
:   Absolute maximum distance value (see **Remarks**)

*DistanceAbsLowerLimit*
:   Absolute minimum distance value (see **Remarks**)

*FirstArcCondition*
:   First arc condition as defined in swDistanceMateArcConditions\_e; valid only for cylindrical distance mates (see **Remarks**)

*SecondArcCondition*
:   Second arc condition as defined in swDistanceMateArcConditions\_e; valid only for cylindrical distance mates (see **Remarks**)

*ErrorStatus*
:   Success or error as defined by swAddMateError\_e

Adds a distance mate to this assembly.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddDistanceMate( _    ByVal AlignFromEnum As System.Integer, _    ByVal Flip As System.Boolean, _    ByVal Distance As System.Double, _    ByVal DistanceAbsUpperLimit As System.Double, _    ByVal DistanceAbsLowerLimit As System.Double, _    ByVal FirstArcCondition As System.Integer, _    ByVal SecondArcCondition As System.Integer, _    ByRef ErrorStatus As System.Integer _ ) As Mate2 ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAssemblyDoc Dim AlignFromEnum As System.Integer Dim Flip As System.Boolean Dim Distance As System.Double Dim DistanceAbsUpperLimit As System.Double Dim DistanceAbsLowerLimit As System.Double Dim FirstArcCondition As System.Integer Dim SecondArcCondition As System.Integer Dim ErrorStatus As System.Integer Dim value As Mate2   value = instance.AddDistanceMate(AlignFromEnum, Flip, Distance, DistanceAbsUpperLimit, DistanceAbsLowerLimit, FirstArcCondition, SecondArcCondition, ErrorStatus) ``` | |

| C# |  |
| --- | --- |
| ``` Mate2 AddDistanceMate(     System.int AlignFromEnum,    System.bool Flip,    System.double Distance,    System.double DistanceAbsUpperLimit,    System.double DistanceAbsLowerLimit,    System.int FirstArcCondition,    System.int SecondArcCondition,    out System.int ErrorStatus ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` Mate2^ AddDistanceMate(  &   System.int AlignFromEnum, &   System.bool Flip, &   System.double Distance, &   System.double DistanceAbsUpperLimit, &   System.double DistanceAbsLowerLimit, &   System.int FirstArcCondition, &   System.int SecondArcCondition, &   [Out] System.int ErrorStatus ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*AlignFromEnum*
:   Type of alignment as defined in swMateAlign\_e

*Flip*
:   True to flip mate entities, false to not (see **Remarks**)

*Distance*
:   Distance value (see **Remarks**)

*DistanceAbsUpperLimit*
:   Absolute maximum distance value (see **Remarks**)

*DistanceAbsLowerLimit*
:   Absolute minimum distance value (see **Remarks**)

*FirstArcCondition*
:   First arc condition as defined in swDistanceMateArcConditions\_e; valid only for cylindrical distance mates (see **Remarks**)

*SecondArcCondition*
:   Second arc condition as defined in swDistanceMateArcConditions\_e; valid only for cylindrical distance mates (see **Remarks**)

*ErrorStatus*
:   Success or error as defined by swAddMateError\_e

#### Return Value

[IMate2](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AssemblyDoc::AddDistanceMate.

# ![](dotnetimages/collapse.gif)Example

[Add and Edit Distance Mate (VBA)](Add_and_Edit_Distance_Mate_Example_VB.htm)

[Add and Edit Distance Mate (VB.NET)](Add_and_Edit_Distance_Mate_Example_VBNET.htm)

[Add and Edit Distance Mate (C#)](Add_and_Edit_Distance_Mate_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

To specify a distance mate without limits, set the DistanceAbsUpperLimit and DistanceAbsLowerLimit parameters equal to the Distance parameter.

If the mate is applied to the closest position that meets the mate condition specified by Distance, then setting Flip to true moves the components to the other possible mate position.

For cylindrical distance mates only, the following FirstArcCondition-to-SecondArcCondition distance combinations are possible:

| FirstArcCondition as defined in swDistanceMateArcConditions\_e | to | SecondArcCondition as defined in swDistanceMateArcConditions\_e |
| --- | --- | --- |
| swArcCondition\_Center |  | swArcCondition\_Center |
| swArcCondition\_Center |  | swArcCondition\_Minimum |
| swArcCondition\_Center |  | swArcCondition\_Maximum |
| swArcCondition\_Minimum |  | swArcCondition\_Center |
| swArcCondition\_Minimum |  | swArcCondition\_Minimum |
| swArcCondition\_Minimum |  | swArcCondition\_Maximum |
| swArcCondition\_Maximum |  | swArcCondition\_Center |
| swArcCondition\_Maximum |  | swArcCondition\_Minimum |
| swArcCondition\_Maximum |  | swArcCondition\_Maximum |

To add a distance mate:

1. Call [IModelDocExtension::SelectByRay](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SelectByRay.html) and [ISelectionMgr::GetSelectedObject6](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISelectionMgr~GetSelectedObject6.html) to get each mate entity. (For cylindrical distance mates, the selections must be two cylindrical faces or one cylindrical face and one axis.)

   - Call [IModelDoc2::ClearSelection2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IModelDoc2~ClearSelection2.html).

     - Call [IEntity::Select4](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IEntity~Select4.html) to select each entity.

       - Call this method.

         - Call [IModelDoc2::EditRebuild3](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDoc2~EditRebuild3.html) after the mate is created.

If entities are not preselected, then ErrorStatus is swAddMateError\_e.swAddMateError\_IncorrectSelections, and nothing is returned.

# ![](dotnetimages/collapse.gif)See Also

####

[IAssemblyDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc.html)

[IAssemblyDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc_members.html)

[IAssemblyDoc::AddMate5 Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~AddMate5.html)

[IAssemblyDoc::EditDistanceMate Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAssemblyDoc~EditDistanceMate.html)

[IMate2::DistanceFirstArcCondition Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~DistanceFirstArcCondition.html)

[IMate2::DistanceSecondArcCondition Property ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IMate2~DistanceSecondArcCondition.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0