<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym~SetDatumTargetRotational.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetDatumTargetRotational Method (IDatumTargetSym) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDatumTargetSym Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym.html) : SetDatumTargetRotational Method (IDatumTargetSym) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*MoveableDatumDirection*
:   Moveable datum direction as defined in swMoveableDatumDirection\_e

*LockLeader*
:   True to lock the leader, false to not

*LockLeaderAngle*
:   Angle of locked leader; valid only if LockLeader is set to true

*GeometryRef*
:   True to use a geometry reference, false to not; true is valid only if MoveableDatumDirection is set to swMoveableDatumDirection\_e.swMoveableDatumDirectionBySelection

*RefGeometryError*
:   Reference geometry error as defined in swRefGeometryError\_e

Sets this datum target to moveable rotational.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetDatumTargetRotational( _    ByVal MoveableDatumDirection As System.Integer, _    ByVal LockLeader As System.Boolean, _    ByVal LockLeaderAngle As System.Double, _    ByVal GeometryRef As System.Boolean, _    ByRef RefGeometryError As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDatumTargetSym Dim MoveableDatumDirection As System.Integer Dim LockLeader As System.Boolean Dim LockLeaderAngle As System.Double Dim GeometryRef As System.Boolean Dim RefGeometryError As System.Integer Dim value As System.Boolean   value = instance.SetDatumTargetRotational(MoveableDatumDirection, LockLeader, LockLeaderAngle, GeometryRef, RefGeometryError) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetDatumTargetRotational(     System.int MoveableDatumDirection,    System.bool LockLeader,    System.double LockLeaderAngle,    System.bool GeometryRef,    out System.int RefGeometryError ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetDatumTargetRotational(  &   System.int MoveableDatumDirection, &   System.bool LockLeader, &   System.double LockLeaderAngle, &   System.bool GeometryRef, &   [Out] System.int RefGeometryError ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*MoveableDatumDirection*
:   Moveable datum direction as defined in swMoveableDatumDirection\_e

*LockLeader*
:   True to lock the leader, false to not

*LockLeaderAngle*
:   Angle of locked leader; valid only if LockLeader is set to true

*GeometryRef*
:   True to use a geometry reference, false to not; true is valid only if MoveableDatumDirection is set to swMoveableDatumDirection\_e.swMoveableDatumDirectionBySelection

*RefGeometryError*
:   Reference geometry error as defined in swRefGeometryError\_e

#### Return Value

True if datum target successfully set, false if errors

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DatumTargetSym::SetDatumTargetRotational.

# ![](dotnetimages/collapse.gif)Remarks

If GeometryRef is set to true, then select a geometry reference before calling this method.

# ![](dotnetimages/collapse.gif)See Also

####

[IDatumTargetSym Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym.html)

[IDatumTargetSym Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym_members.html)

[IDatumTargetSym::SetDatumTargetNotMoveable Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym~SetDatumTargetNotMoveable.html)

[IDatumTargetSym::SetDatumTargetHorizontal Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym~SetDatumTargetHorizontal.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0