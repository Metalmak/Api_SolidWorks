<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTrendTracker~SetBaseLine.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| SetBaseLine Method (ICWTrendTracker) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWTrendTracker Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTrendTracker.html) : SetBaseLine Method (ICWTrendTracker) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Sets the current results as the baseline for weight, displacement, stress, etc.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetBaseLine() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWTrendTracker Dim value As System.Integer   value = instance.SetBaseLine() ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetBaseLine() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetBaseLine(); ``` | |

#### Return Value

Error code as defined in [swsTrendTrackerErrorCode\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTrendTrackerErrorCode_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWTrendTracker::SetBaseLine.

# ![](dotnetimages/collapse.gif)Example

See the [ICWTrendTracker](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTrendTracker.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWTrendTracker Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTrendTracker.html)

[ICWTrendTracker Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWTrendTracker_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2016 SP0