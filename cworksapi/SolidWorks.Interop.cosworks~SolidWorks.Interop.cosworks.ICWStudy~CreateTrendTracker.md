<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~CreateTrendTracker.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| CreateTrendTracker Method (ICWStudy) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html) : CreateTrendTracker Method (ICWStudy) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ErrorCode*
:   Error code as defined in [swsTrendTrackerErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTrendTrackerErrorCode_e.html)

Creates a Trend Tracker for this study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function CreateTrendTracker( _    ByRef ErrorCode As System.Integer _ ) As CWTrendTracker ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudy Dim ErrorCode As System.Integer Dim value As CWTrendTracker   value = instance.CreateTrendTracker(ErrorCode) ``` | |

| C# |  |
| --- | --- |
| ``` CWTrendTracker CreateTrendTracker(     out System.int ErrorCode ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` CWTrendTracker^ CreateTrendTracker(  &   [Out] System.int ErrorCode ) ``` | |

#### Parameters

*ErrorCode*
:   Error code as defined in [swsTrendTrackerErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTrendTrackerErrorCode_e.html)

#### Return Value

[ICWTrendTracker](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTrendTracker.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudy::CreateTrendTracker.

# ![](dotnetimages/collapse.gif)Example

[Create Trend Tracker (VBA)](Create_Trend_Tracker_Example_VB.htm)

[Create Trend Tracker (VB.NET)](Create_Trend_Tracker_Example_VBNET.htm)

[Create Trend Tracker (C#)](Create_Trend_Tracker_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html)

[ICWStudy Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy_members.html)

[ICWStudy::DeleteTrendTracker Method ()](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~DeleteTrendTracker.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0