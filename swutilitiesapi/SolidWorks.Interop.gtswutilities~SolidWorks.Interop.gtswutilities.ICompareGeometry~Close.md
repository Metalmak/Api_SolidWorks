<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareGeometry~Close.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| Close Method (ICompareGeometry) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [ICompareGeometry Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareGeometry.html) : Close Method (ICompareGeometry) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Performs any necessary cleanup after the geometry in the documents have been compared.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Close() As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICompareGeometry Dim value As System.Integer   value = instance.Close() ``` | |

| C# |  |
| --- | --- |
| ``` System.int Close() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int Close(); ``` | |

#### Return Value

Error as defined by [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ICompareGeometry::Close.

# ![](dotnetimages/collapse.gif)Example

[Compare Geometry (VBA)](Compare_Geometry_VB6.htm)

[Set Tolerances and Compare Geometry (VBA)](Set_Tolerances_and_Compare_Geometry_VB6.htm)

[Compare Geometry (VB.NET)](Compare_Geometry_VBNET.htm)

[Compare Geometry (C#)](Compare_Geometry_CSharp.htm)

[Set Tolerances and Compare Geometry (VB.NET)](Set_Tolerances_and_Compare_Geometry_VBNET.htm)

[Set Tolerances and Compare Geometry (C#)](Set_Tolerances_and_Compare_Geometry_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICompareGeometry Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareGeometry.html)

[ICompareGeometry Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.ICompareGeometry_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2004 FCS