<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym~SetDatumTargetHorizontal.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetDatumTargetHorizontal Method (IDatumTargetSym) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IDatumTargetSym Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym.html) : SetDatumTargetHorizontal Method (IDatumTargetSym) |

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

Sets this datum target to moveable horizontal.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetDatumTargetHorizontal( _    ByVal MoveableDatumDirection As System.Integer, _    ByVal LockLeader As System.Boolean, _    ByVal LockLeaderAngle As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDatumTargetSym Dim MoveableDatumDirection As System.Integer Dim LockLeader As System.Boolean Dim LockLeaderAngle As System.Double Dim value As System.Boolean   value = instance.SetDatumTargetHorizontal(MoveableDatumDirection, LockLeader, LockLeaderAngle) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetDatumTargetHorizontal(     System.int MoveableDatumDirection,    System.bool LockLeader,    System.double LockLeaderAngle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetDatumTargetHorizontal(  &   System.int MoveableDatumDirection, &   System.bool LockLeader, &   System.double LockLeaderAngle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*MoveableDatumDirection*
:   Moveable datum direction as defined in swMoveableDatumDirection\_e

*LockLeader*
:   True to lock the leader, false to not

*LockLeaderAngle*
:   Angle of locked leader; valid only if LockLeader is set to true

#### Return Value

True if this datum target is successfully set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DatumTargetSym::SetDatumTargetHorizontal.

# ![](dotnetimages/collapse.gif)See Also

####

[IDatumTargetSym Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym.html)

[IDatumTargetSym Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym_members.html)

[IDatumTargetSym::SetDatumTargetNotMoveable Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym~SetDatumTargetNotMoveable.html)

[IDatumTargetSym::SetDatumTargetRotational Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IDatumTargetSym~SetDatumTargetRotational.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2018 FCS, Revision Number 26.0