<!-- source: swutilitiesapi/SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IUtilOptions~SetAngularTolerance.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Utilities API Help | Send comments on this topic. |
| SetAngularTolerance Method (IUtilOptions) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.gtswutilities Namespace](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities_namespace.html) > [IUtilOptions Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IUtilOptions.html) : SetAngularTolerance Method (IUtilOptions) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*pTol*
:   Angular tolerance

Sets the angular tolerance for the face comparison.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetAngularTolerance( _    ByVal pTol As System.Double _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IUtilOptions Dim pTol As System.Double Dim value As System.Integer   value = instance.SetAngularTolerance(pTol) ``` | |

| C# |  |
| --- | --- |
| ``` System.int SetAngularTolerance(     System.double pTol ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int SetAngularTolerance(  &   System.double pTol ) ``` | |

#### Parameters

*pTol*
:   Angular tolerance

#### Return Value

Error as defined by [gtError\_e](SOLIDWORKS.Interop.gtswutilities~SOLIDWORKS.Interop.gtswutilities.gtError_e.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See IUtilOptions::SetAngularTolerance.

# ![](dotnetimages/collapse.gif)Example

[Set Tolerances and Compare Geometry (VBA)](Set_Tolerances_and_Compare_Geometry_VB6.htm)

[Set Tolerances and Compare Geometry (VB.NET)](Set_Tolerances_and_Compare_Geometry_VBNET.htm)

[Set Tolerances and Compare Geometry (C#)](Set_Tolerances_and_Compare_Geometry_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

During face comparison, the parallelism of the edges of face pairs are compared. If the edges are curved, tangents to the curves are compared. The faces are identical if the angle between their corresponding edges is less than the specified angle tolerance.

# ![](dotnetimages/collapse.gif)See Also

####

[IUtilOptions Interface](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IUtilOptions.html)

[IUtilOptions Members](SolidWorks.Interop.gtswutilities~SolidWorks.Interop.gtswutilities.IUtilOptions_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS Utilities API 2004 FCS