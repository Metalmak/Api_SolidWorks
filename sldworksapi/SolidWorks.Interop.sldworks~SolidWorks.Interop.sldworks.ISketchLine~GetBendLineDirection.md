<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchLine~GetBendLineDirection.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetBendLineDirection Method (ISketchLine) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchLine Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchLine.html) : GetBendLineDirection Method (ISketchLine) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets whether the sketch line is a bendline, and, if it is, the direction of the bendline.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetBendLineDirection() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchLine Dim value As System.Integer   value = instance.GetBendLineDirection() ``` | |

| C# |  |
| --- | --- |
| ``` System.int GetBendLineDirection() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int GetBendLineDirection(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Bendline direction as defined in swBendLineDirection\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchLine::GetBendLineDirection.

# ![](dotnetimages/collapse.gif)Example

[Get Direction of Bendline (C#)](Get_Direction_of_Bendline_Example_CSharp.htm)

[Get Direction of Bendline (VB.NET)](Get_Direction_of_Bendline_Example_VBNET.htm)

[Get Direction of Bendline (VBA)](Get_Direction_of_Bendline_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchLine Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchLine.html)

[ISketchLine Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchLine_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0