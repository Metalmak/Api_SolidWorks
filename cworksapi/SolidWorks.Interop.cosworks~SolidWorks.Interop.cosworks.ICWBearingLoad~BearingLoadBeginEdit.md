<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad~BearingLoadBeginEdit.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| BearingLoadBeginEdit Method (ICWBearingLoad) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWBearingLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad.html) : BearingLoadBeginEdit Method (ICWBearingLoad) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Starts editing a bearing load.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub BearingLoadBeginEdit() ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWBearingLoad   instance.BearingLoadBeginEdit() ``` | |

| C# |  |
| --- | --- |
| ``` void BearingLoadBeginEdit() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void BearingLoadBeginEdit(); ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWBearingLoad::BearingLoadBeginEdit.

# ![](dotnetimages/collapse.gif)Example

See the [ICWBearingLoad](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

To start editing a bearing load, you must call this method. You must call [ICWBearingLoad::BearingLoadEndEdit](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWBearingLoad~BearingLoadEndEdit.html) to end editing that bearing load. Changes are not applied unless you call both methods.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWBearingLoad Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad.html)

[ICWBearingLoad Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBearingLoad_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2009 SP0