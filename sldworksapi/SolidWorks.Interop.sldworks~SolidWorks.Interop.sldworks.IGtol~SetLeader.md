<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~SetLeader.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetLeader Method (IGtol) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IGtol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol.html) : SetLeader Method (IGtol) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Leader*
:   True enables a leader on this symbol, false disables it

*LeaderSide*
:   Leader attachment information as defined in swLeaderSide\_e

*BentLeader*
:   True enables a bent leader on this symbol, false disables it

*AllAround*
:   True enables the all around symbol on the leader, false disables it

Sets the characteristics of the leader for this symbol.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetLeader( _    ByVal Leader As System.Boolean, _    ByVal LeaderSide As System.Integer, _    ByVal BentLeader As System.Boolean, _    ByVal AllAround As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IGtol Dim Leader As System.Boolean Dim LeaderSide As System.Integer Dim BentLeader As System.Boolean Dim AllAround As System.Boolean   instance.SetLeader(Leader, LeaderSide, BentLeader, AllAround) ``` | |

| C# |  |
| --- | --- |
| ``` void SetLeader(     System.bool Leader,    System.int LeaderSide,    System.bool BentLeader,    System.bool AllAround ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetLeader(  &   System.bool Leader, &   System.int LeaderSide, &   System.bool BentLeader, &   System.bool AllAround ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Leader*
:   True enables a leader on this symbol, false disables it

*LeaderSide*
:   Leader attachment information as defined in swLeaderSide\_e

*BentLeader*
:   True enables a bent leader on this symbol, false disables it

*AllAround*
:   True enables the all around symbol on the leader, false disables it

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Gtol::SetLeader.

# ![](dotnetimages/collapse.gif)Remarks

This method ignores:

* LeaderSide, BentLeader, and AllAround values if the leader value is false. Use [IGtol::IsAttached](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IGtol~IsAttached.html) to determine if this symbol is currently using a leader.

  * AllAround value if the BentLeader value is false. Use [IGtol::HasExtraLeader](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IGtol~HasExtraLeader.html) to determine if this symbol is using a bent leader.

Use:

* [IGtol::GetLeaderSide](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IGtol~GetLeaderSide.html) to determine where the leader is attached to the symbol

  * [IGtol::GetAllAround](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IGtol~GetAllAround.html) to determine if this leader is using the all around symbol

# ![](dotnetimages/collapse.gif)See Also

####

[IGtol Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol.html)

[IGtol Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol_members.html)

[IGtol::GetLeaderAtIndex2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~GetLeaderAtIndex2.html)

[IGtol::GetLeaderCount Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~GetLeaderCount.html)

[IGtol::GetLeaderInfo Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~GetLeaderInfo.html)

[IGtol::IGetLeaderAtIndex2 Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~IGetLeaderAtIndex2.html)

[IGtol::IGetLeaderInfo Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IGtol~IGetLeaderInfo.html)