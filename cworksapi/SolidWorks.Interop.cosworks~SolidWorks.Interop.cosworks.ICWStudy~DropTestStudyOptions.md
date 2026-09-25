<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~DropTestStudyOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| DropTestStudyOptions Property (ICWStudy) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html) : DropTestStudyOptions Property (ICWStudy) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the options for this drop test study.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property DropTestStudyOptions As CWDropTestStudyOptions ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWStudy Dim value As CWDropTestStudyOptions   value = instance.DropTestStudyOptions ``` | |

| C# |  |
| --- | --- |
| ``` CWDropTestStudyOptions DropTestStudyOptions {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property CWDropTestStudyOptions^ DropTestStudyOptions {    CWDropTestStudyOptions^ get(); } ``` | |

#### Property Value

[ICWDropTestStudyOptions](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWDropTestStudyOptions.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWStudy::DropTestStudyOptions.

# ![](dotnetimages/collapse.gif)Example

[Create Drop Test Study (VBA)](Create_Drop_Test_Study_Example_VB.htm)

[Create Drop Test Study (VB.NET)](Create_Drop_Test_Study_Example_VBNET.htm)

[Create Drop Test Study (C#)](Create_Drop_Test_Study_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWStudy Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy.html)

[ICWStudy Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy_members.html)

[ICWStudy::AddDropTestSetup Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~AddDropTestSetup.html)

[ICWStudy::DropTestResultOptions Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~DropTestResultOptions.html)

[ICWStudy::DropTestSetup Property](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWStudy~DropTestSetup.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2012 SP0