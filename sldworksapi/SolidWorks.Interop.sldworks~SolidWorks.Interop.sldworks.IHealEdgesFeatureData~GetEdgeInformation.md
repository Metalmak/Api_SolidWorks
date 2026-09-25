<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHealEdgesFeatureData~GetEdgeInformation.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetEdgeInformation Method (IHealEdgesFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IHealEdgesFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHealEdgesFeatureData.html) : GetEdgeInformation Method (IHealEdgesFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*EdgeCountBefore*
:   Number of edges before healing

*EdgeCountAfter*
:   Number of edges after healing

Gets the number of edges before healing and the number of edges after healing.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub GetEdgeInformation( _    ByRef EdgeCountBefore As System.Integer, _    ByRef EdgeCountAfter As System.Integer _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IHealEdgesFeatureData Dim EdgeCountBefore As System.Integer Dim EdgeCountAfter As System.Integer   instance.GetEdgeInformation(EdgeCountBefore, EdgeCountAfter) ``` | |

| C# |  |
| --- | --- |
| ``` void GetEdgeInformation(     out System.int EdgeCountBefore,    out System.int EdgeCountAfter ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void GetEdgeInformation(  &   [Out] System.int EdgeCountBefore, &   [Out] System.int EdgeCountAfter ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*EdgeCountBefore*
:   Number of edges before healing

*EdgeCountAfter*
:   Number of edges after healing

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See HealEdgesFeatureData::GetEdgeInformation.

# ![](dotnetimages/collapse.gif)Example

[Modify Heal Edges Feature (VBA)](Modify_Heal_Edges_Feature_Example_VB.htm)

[Get Heal Edges Feature Data (C#)](Get_Heal_Edges_Feature_Data_Example_CSharp.htm)

[Get Heal Edges Feature Data (VB.NET)](Get_Heal_Edges_Feature_Data_Example_VBNET.htm)

[Get Heal Edges Feature Data (VBA)](Get_Heal_Edges_Feature_Data_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IHealEdgesFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHealEdgesFeatureData.html)

[IHealEdgesFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IHealEdgesFeatureData_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0