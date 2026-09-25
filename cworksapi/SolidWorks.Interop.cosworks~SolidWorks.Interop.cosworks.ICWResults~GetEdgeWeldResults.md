<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults~GetEdgeWeldResults.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| GetEdgeWeldResults Method (ICWResults) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html) : GetEdgeWeldResults Method (ICWResults) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*EdgeWeldConnector*
:   Name of the edge weld connector for which to get edge weld results

*NUnit*
:   Unit as defined in [swsUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUnit_e.html)

*BPassFail*
:   True if the edge weld is safe to use, false if not

*ErrorCode*
:   Error code as defined in [swsWeldResultErrorCode\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsWeldResultErrorCode_e.html)

Gets the edge weld results for the specified edge weld connector.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetEdgeWeldResults( _    ByVal EdgeWeldConnector As System.String, _    ByVal NUnit As System.Integer, _    ByRef BPassFail As System.Boolean, _    ByRef ErrorCode As System.Integer _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWResults Dim EdgeWeldConnector As System.String Dim NUnit As System.Integer Dim BPassFail As System.Boolean Dim ErrorCode As System.Integer Dim value As System.Object   value = instance.GetEdgeWeldResults(EdgeWeldConnector, NUnit, BPassFail, ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` System.object GetEdgeWeldResults(     System.string EdgeWeldConnector,    System.int NUnit,    out System.bool BPassFail,    out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ GetEdgeWeldResults(  &   System.String^ EdgeWeldConnector, &   System.int NUnit, &   [Out] System.bool BPassFail, &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*EdgeWeldConnector*
:   Name of the edge weld connector for which to get edge weld results

*NUnit*
:   Unit as defined in [swsUnit\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsUnit_e.html)

*BPassFail*
:   True if the edge weld is safe to use, false if not

*ErrorCode*
:   Error code as defined in [swsWeldResultErrorCode\_e](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.swsWeldResultErrorCode_e.html)

#### Return Value

Array of edge weld results (see **Remarks**)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWResults::GetEdgeWeldResults.

# ![](dotnetimages/collapse.gif)Example

[Calculate Edge Weld Results (C#)](Calculate_Edge_Weld_Results_Example_CSharp.htm)

[Calculate Edge Weld Results (VB.NET)](Calculate_Edge_Weld_Results_Example_VBNET.htm)

[Calculate Edge Weld Results (VBA)](Calculate_Edge_Weld_Results_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

The array of edge weld results contains these minimum, maximum, and mean values in this order:

* Weld size* Weld throat size* Joint normal force* Shear-weld axis force* Shear-surface normal force* Bending moment

# ![](dotnetimages/collapse.gif)See Also

####

[ICWResults Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults.html)

[ICWResults Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWResults_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2013 SP3.0