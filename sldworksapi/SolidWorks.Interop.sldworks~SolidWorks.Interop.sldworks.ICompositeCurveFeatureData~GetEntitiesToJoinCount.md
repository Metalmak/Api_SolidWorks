<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICompositeCurveFeatureData~GetEntitiesToJoinCount.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetEntitiesToJoinCount Method (ICompositeCurveFeatureData) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICompositeCurveFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICompositeCurveFeatureData.html) : GetEntitiesToJoinCount Method (ICompositeCurveFeatureData) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the number of entities that are joined to create a composite curve.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetEntitiesToJoinCount() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICompositeCurveFeatureData Dim value As System.Integer   value = instance.GetEntitiesToJoinCount() ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetEntitiesToJoinCount() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetEntitiesToJoinCount(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Number of entities

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CompositeCurveFeatureData::GetEntitiesToJoinCount.

# ![](dotnetimages/collapse.gif)Example

[Insert a Composite Curve (C#)](Insert_a_Composite_Curve_Example_CSharp.htm)

[Insert a Composite Curve (VB.NET)](Insert_a_Composite_Curve_Example_VBNET.htm)

[Insert a Composite Curve (VBA)](Insert_a_Composite_Curve_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Call this method before calling [ICompositeCurveFeatureData::IGetEntitiesToJoin](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICompositeCurveFeatureData~IGetEntitiesToJoin.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ICompositeCurveFeatureData Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICompositeCurveFeatureData.html)

[ICompositeCurveFeatureData Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICompositeCurveFeatureData_members.html)

[ICompositeCurveFeatureData::GetEntitiesToJoin Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICompositeCurveFeatureData~GetEntitiesToJoin.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2003 FCS, Revision Number 11.0