<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData~UnChainMemberPairs.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| UnChainMemberPairs Property (ISecondaryMemberBetweenPointsFeatureData) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISecondaryMemberBetweenPointsFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData.html) : UnChainMemberPairs Property (ISecondaryMemberBetweenPointsFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets and sets whether to chain member pairs to create this secondary structure system member.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property UnChainMemberPairs As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISecondaryMemberBetweenPointsFeatureData Dim value As System.Boolean   instance.UnChainMemberPairs = value   value = instance.UnChainMemberPairs ``` | |

| C# |  |
| --- | --- |
| ``` System.bool UnChainMemberPairs {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool UnChainMemberPairs {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to pair each member passed in [ISecondaryMemberBetweenPointsFeatureData::SetMemberPairs](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData~SetMemberPairs.html) to the previous member passed, false to pair consecutive members only

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SecondaryMemberBetweenPointsFeatureData::UnChainMemberPairs.

# ![](dotnetimages/collapse.gif)Remarks

If this property is set to true, each primary member passed to ISecondaryMemberBetweenPointsFeatureData::SetMemberPairs pairs with the previous primary member to create a new member pair.

For the list of members A,B,C,D,E,F:

If this property is set to true, then 5 member pairs are created:

A -- B

B -- C

C -- D

D -- E

E -- F

If this property is set to false, then only 3 member pairs are created:

A -- B

C -- D

E -- F

# ![](dotnetimages/collapse.gif)See Also

####

[ISecondaryMemberBetweenPointsFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData.html)

[ISecondaryMemberBetweenPointsFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISecondaryMemberBetweenPointsFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2022 FCS, Revision Number 30