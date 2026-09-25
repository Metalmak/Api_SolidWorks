<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICosmosWorks~ActiveDoc.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ActiveDoc Property (ICosmosWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) > [ICosmosWorks Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICosmosWorks.html) : ActiveDoc Property (ICosmosWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the model document.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` ReadOnly Property ActiveDoc As CWModelDoc ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICosmosWorks Dim value As CWModelDoc   value = instance.ActiveDoc ``` | |

| C# |  |
| --- | --- |
| ``` CWModelDoc ActiveDoc {get;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property CWModelDoc^ ActiveDoc {    CWModelDoc^ get(); } ``` | |

#### Property Value

[Model document](SOLIDWORKS.Interop.cosworks~SOLIDWORKS.Interop.cosworks.ICWModelDoc.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CosmosWorks::ActiveDoc.

# ![](dotnetimages/collapse.gif)Example

[Create Nonlinear Study and Apply Materials (C#)](Create_Nonlinear_Study_and_Apply_Materials_Example_CSharp.htm)

[Create Nonlinear Study and Apply Materials (VB.NET)](Create_Nonlinear_Study_and_Apply_Materials_Example_VBNET.htm)

[Create Nonlinear Study and Apply Materials (VBA)](Create_Nonlinear_Study_and_Apply_Materials_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICosmosWorks Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICosmosWorks.html)

[ICosmosWorks Members](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICosmosWorks_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Simulation API 2008 SP1.0