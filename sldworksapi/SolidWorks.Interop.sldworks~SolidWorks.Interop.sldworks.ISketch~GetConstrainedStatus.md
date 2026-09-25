<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~GetConstrainedStatus.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetConstrainedStatus Method (ISketch) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketch Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html) : GetConstrainedStatus Method (ISketch) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the current constrained status of the sketch.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetConstrainedStatus() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketch Dim value As System.Integer   value = instance.GetConstrainedStatus() ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetConstrainedStatus() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetConstrainedStatus(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Constrained status as defined in swConstrainedStatus\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Sketch::GetConstrainedStatus.

# ![](dotnetimages/collapse.gif)Example

[Get Sketch Constraints (VBA)](Get_Sketch_Constraints_Example_VB.htm)

[Autodimension All Sketches (C#)](Autodimension_All_Sketches_Example_CSharp.htm)

[Autodimension All Sketches (VB.NET)](Autodimension_All_Sketches_Example_VBNET.htm)

[Autodimension All Sketches (VBA)](Autodimension_All_Sketches_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISketch Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch.html)

[ISketch Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch_members.html)

[ISketch::ConstrainAll Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketch~ConstrainAll.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2000 FCS, Revision Number 8.0