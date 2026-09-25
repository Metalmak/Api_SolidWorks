<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertCompoundWidthFeature~GetNominalCompoundWidth.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| GetNominalCompoundWidth Method (IDimXpertCompoundWidthFeature) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertCompoundWidthFeature Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertCompoundWidthFeature.html) : GetNominalCompoundWidth Method (IDimXpertCompoundWidthFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Width*
:   Width of the feature

*X*
:   X-coordinate of the width

*Y*
:   Y-coordinate of the width

*Z*
:   Z-coordinate of the width

*I*
:   I component of the direction vector of the width

*J*
:   J component of the direction vector of the width

*K*
:   K component of the direction vector of the width

Gets various attributes for this DimXpert compound width.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetNominalCompoundWidth( _    ByRef Width As System.Double, _    ByRef X As System.Double, _    ByRef Y As System.Double, _    ByRef Z As System.Double, _    ByRef I As System.Double, _    ByRef J As System.Double, _    ByRef K As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertCompoundWidthFeature Dim Width As System.Double Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim I As System.Double Dim J As System.Double Dim K As System.Double Dim value As System.Boolean   value = instance.GetNominalCompoundWidth(Width, X, Y, Z, I, J, K) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetNominalCompoundWidth(     out System.double Width,    out System.double X,    out System.double Y,    out System.double Z,    out System.double I,    out System.double J,    out System.double K ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetNominalCompoundWidth(  &   [Out] System.double Width, &   [Out] System.double X, &   [Out] System.double Y, &   [Out] System.double Z, &   [Out] System.double I, &   [Out] System.double J, &   [Out] System.double K ) ``` | |

#### Parameters

*Width*
:   Width of the feature

*X*
:   X-coordinate of the width

*Y*
:   Y-coordinate of the width

*Z*
:   Z-coordinate of the width

*I*
:   I component of the direction vector of the width

*J*
:   J component of the direction vector of the width

*K*
:   K component of the direction vector of the width

#### Return Value

True if method call is successful; false otherwise

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimXpertCompoundWidthFeature::GetNominalCompoundWidth.

# ![](dotnetimages/collapse.gif)Example

[Get and Set Size Dimension Example (C#)](Get_and_Set_Size_Dimension_Example_CSharp.htm)

[Get and Set Size Dimension Example (VB.NET)](Get_and_Set_Size_Dimension_Example_VBNET.htm)

[Get and Set Size Dimension Example (VBA)](Get_and_Set_Size_Dimension_Example_VB.htm)

[Get DimXpert Width And Best Fit Plane Features Example (VBA)](Get_DimXpert_Width_And_BestFitPlane_Features_Example_VB.htm)

[Get DimXpert Width And Best Fit Plane Features Example (VB.NET)](Get_DimXpert_Width_And_BestFitPlane_Features_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertCompoundWidthFeature Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertCompoundWidthFeature.html)

[IDimXpertCompoundWidthFeature Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertCompoundWidthFeature_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0