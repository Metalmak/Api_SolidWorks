<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IUtilOptions~SetPositionTolerance.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| SetPositionTolerance Method (IUtilOptions) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [IUtilOptions Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IUtilOptions.html) : SetPositionTolerance Method (IUtilOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*pTol*
:   Position tolerance

Sets the position tolerance for the face comparison.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetPositionTolerance( _    ByVal pTol As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IUtilOptions Dim pTol As System.Double Dim value As System.Integer   value = instance.SetPositionTolerance(pTol) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetPositionTolerance(     System.double pTol ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetPositionTolerance(  &   System.double pTol ) ``` | |

#### Parameters

*pTol*
:   Position tolerance

#### Return Value

Error as defined by [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See IUtilOptions::SetPositionTolerance.

# ![](dotnetimages/collapse.gif)Example

[Set Tolerances and Compare Geometry (VBA)](Set_Tolerances_and_Compare_Geometry_VB6.htm)

[Set Tolerances and Compare Geometry (VB.NET)](Set_Tolerances_and_Compare_Geometry_VBNET.htm)

[Set Tolerances and Compare Geometry (C#)](Set_Tolerances_and_Compare_Geometry_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

During face comparison, the position of vertex coordinates and some surface points of face pairs are compared. Vertices or points that lie within a specified position tolerance are considered identical.

# ![](dotnetimages/collapse.gif)See Also

####

[IUtilOptions Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IUtilOptions.html)

[IUtilOptions Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IUtilOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2004 FCS