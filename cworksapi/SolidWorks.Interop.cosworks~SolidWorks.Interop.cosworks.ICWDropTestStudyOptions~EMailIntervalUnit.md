<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestStudyOptions~EMailIntervalUnit.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| EMailIntervalUnit Property (ICWDropTestStudyOptions) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWDropTestStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestStudyOptions.html) : EMailIntervalUnit Property (ICWDropTestStudyOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets the units of time for [ICWDropTestStudyOptions::EMailInterval](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestStudyOptions~EMailInterval.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property EMailIntervalUnit As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWDropTestStudyOptions Dim value As System.Integer   instance.EMailIntervalUnit = value   value = instance.EMailIntervalUnit ``` | |

| C# |  |
| --- | --- |
| ``` System.int EMailIntervalUnit {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.int EMailIntervalUnit {    System.int get();    void set ( &   System.int value); } ``` | |

#### Property Value

Time units as defined in [swsTimeUnits\_e](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.swsTimeUnits_e.html):

* swsSecond* swsMinute* swsHour

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWDropTestStudyOptions::EMailIntervalUnit.

# ![](dotnetimages/collapse.gif)Remarks

This property is valid only if:

* [ICWDropTestStudyOptions::EMailTimebased](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestStudyOptions~EMailTimebased.html) is set to 1,

    - and -

* [ICWDropTestStudyOptions::EMail](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestStudyOptions~EMail.html) is set to 1.

# ![](dotnetimages/collapse.gif)See Also

####

[ICWDropTestStudyOptions Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestStudyOptions.html)

[ICWDropTestStudyOptions Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWDropTestStudyOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2018 SP0