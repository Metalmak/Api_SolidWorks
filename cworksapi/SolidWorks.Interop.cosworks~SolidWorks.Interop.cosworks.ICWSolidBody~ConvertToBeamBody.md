<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody~ConvertToBeamBody.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ConvertToBeamBody Method (ICWSolidBody) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICWSolidBody Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody.html) : ConvertToBeamBody Method (ICWSolidBody) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Treat a solid body as a beam.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ConvertToBeamBody() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICWSolidBody Dim value As System.Integer   value = instance.ConvertToBeamBody() ``` | |

| C# |  |
| --- | --- |
| ``` System.int ConvertToBeamBody() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int ConvertToBeamBody(); ``` | |

#### Return Value

0 to treat a solid body as a beam, 1 to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CWSolidBody::ConvertToBeamBody.

# ![](dotnetimages/collapse.gif)Example

[Change Beam to Solid Body and Back (C#)](Change_Beam_to_Solid_Body_and_Back_Example_CSharp.htm)

[Change Beam to Solid Body and Back (VB.NET)](Change_Beam_to_Solid_Body_and_Back_Example_VBNET.htm)

[Change Beam to Solid Body and Back (VBA)](Change_Beam_to_Solid_Body_and_Back_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWSolidBody Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody.html)

[ICWSolidBody Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWSolidBody_members.html)

[ICWBeamBody::ConvertToSolidBody Method](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody~ConvertToSolidBody.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2010 SP0