<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IChamferFeatureData2~SetEdgeChamferDistance.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetEdgeChamferDistance Method (IChamferFeatureData2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IChamferFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IChamferFeatureData2.html) : SetEdgeChamferDistance Method (IChamferFeatureData2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Side*
:   Feature direction (see **Remarks**)

*Distance*
:   Edge chamfer distance

Sets the edge chamfer distance on either side of the edge.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetEdgeChamferDistance( _    ByVal Side As System.Integer, _    ByVal Distance As System.Double _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IChamferFeatureData2 Dim Side As System.Integer Dim Distance As System.Double   instance.SetEdgeChamferDistance(Side, Distance) ``` | |

| C# |  |
| --- | --- |
| ``` void SetEdgeChamferDistance(     System.int Side,    System.double Distance ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetEdgeChamferDistance(  &   System.int Side, &   System.double Distance ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Side*
:   Feature direction (see **Remarks**)

*Distance*
:   Edge chamfer distance

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ChamferFeatureData2::SetEdgeChamferDistance.

# ![](dotnetimages/collapse.gif)Remarks

Set the Side parameter to 0 or 1. For angle-distance chamfers, set side to 0.

# ![](dotnetimages/collapse.gif)See Also

####

[IChamferFeatureData2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IChamferFeatureData2.html)

[IChamferFeatureData2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IChamferFeatureData2_members.html)

[IChamferFeatureData2::GetEdgeChamferDistance Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IChamferFeatureData2~GetEdgeChamferDistance.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0