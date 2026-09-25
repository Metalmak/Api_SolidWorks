<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertSphereFeature~GetNominalSphere.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| GetNominalSphere Method (IDimXpertSphereFeature) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertSphereFeature Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertSphereFeature.html) : GetNominalSphere Method (IDimXpertSphereFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*R*
:   Radius of the sphere

*X*
:   X-coordinate of the origin of the sphere

*Y*
:   Y-coordinate of the origin of the sphere

*Z*
:   Z-coordinate of the origin of the sphere

Gets the coordinates and vector for this DimXpert sphere.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetNominalSphere( _    ByRef R As System.Double, _    ByRef X As System.Double, _    ByRef Y As System.Double, _    ByRef Z As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertSphereFeature Dim R As System.Double Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim value As System.Boolean   value = instance.GetNominalSphere(R, X, Y, Z) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetNominalSphere(     out System.double R,    out System.double X,    out System.double Y,    out System.double Z ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetNominalSphere(  &   [Out] System.double R, &   [Out] System.double X, &   [Out] System.double Y, &   [Out] System.double Z ) ``` | |

#### Parameters

*R*
:   Radius of the sphere

*X*
:   X-coordinate of the origin of the sphere

*Y*
:   Y-coordinate of the origin of the sphere

*Z*
:   Z-coordinate of the origin of the sphere

#### Return Value

True if method call is successful; false otherwise

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimXpertSphereFeature::GetNominalSphere.

# ![](dotnetimages/collapse.gif)Example

[Get DimXpert Sphere Feature Example (VBA)](Get_DimXpert_Sphere_Feature_Example_VB.htm)

[Get DimXpert Sphere Feature Example (VB.NET)](Get_DimXpert_Sphere_Feature_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertSphereFeature Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertSphereFeature.html)

[IDimXpertSphereFeature Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertSphereFeature_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0