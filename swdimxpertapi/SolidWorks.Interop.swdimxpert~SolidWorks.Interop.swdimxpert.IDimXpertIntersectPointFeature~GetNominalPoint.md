<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertIntersectPointFeature~GetNominalPoint.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| GetNominalPoint Method (IDimXpertIntersectPointFeature) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertIntersectPointFeature Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertIntersectPointFeature.html) : GetNominalPoint Method (IDimXpertIntersectPointFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*X*
:   X-coordinate of the intersect point

*Y*
:   Y-coordinate of the intersect point

*Z*
:   Z-coordinate of the intersect point

Gets the coordinates of this DimXpert intersect point.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetNominalPoint( _    ByRef X As System.Double, _    ByRef Y As System.Double, _    ByRef Z As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertIntersectPointFeature Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim value As System.Boolean   value = instance.GetNominalPoint(X, Y, Z) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetNominalPoint(     out System.double X,    out System.double Y,    out System.double Z ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetNominalPoint(  &   [Out] System.double X, &   [Out] System.double Y, &   [Out] System.double Z ) ``` | |

#### Parameters

*X*
:   X-coordinate of the intersect point

*Y*
:   Y-coordinate of the intersect point

*Z*
:   Z-coordinate of the intersect point

#### Return Value

True if method call is successful; false otherwise

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimXpertIntersectPointFeature::GetNominalPoint.

# ![](dotnetimages/collapse.gif)Example

[Get DimXpert Intersect Features Example (VBA)](Get_DimXpert_Intersect_Features_Example_VB.htm)

[Get DimXpert Intersect Features Example (VB.NET)](Get_DimXpert_Intersect_Features_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertIntersectPointFeature Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertIntersectPointFeature.html)

[IDimXpertIntersectPointFeature Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertIntersectPointFeature_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0