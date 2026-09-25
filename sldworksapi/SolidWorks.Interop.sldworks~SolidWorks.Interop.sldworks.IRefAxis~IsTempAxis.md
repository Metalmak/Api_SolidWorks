<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis~IsTempAxis.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IsTempAxis Method (IRefAxis) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRefAxis Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis.html) : IsTempAxis Method (IRefAxis) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets whether the reference axis is a temporary axis.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IsTempAxis() As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRefAxis Dim value As System.Boolean   value = instance.IsTempAxis() ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IsTempAxis() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool IsTempAxis(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

True if the reference axis is a temporary axis, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RefAxis::IsTempAxis.

# ![](dotnetimages/collapse.gif)Example

[Get Temporary Axis and Its Reference Face (C#)](Get_Temporary_Axis_and_Its_Reference_Face_Example_CSharp.htm)

[Get Temporary Axis and Its Reference Face (VB.NET)](Get_Temporary_Axis_and_Its_Reference_Face_Example_VBNET.htm)

[Get Temporary Axis and Its Reference Face (VBA)](Get_Temporary_Axis_and_Its_Reference_Face_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IRefAxis Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis.html)

[IRefAxis Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis_members.html)

[IRefAxis::GetTempAxisReferenceFace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRefAxis~GetTempAxisReferenceFace.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2017 FCS, Revision Number 25.0