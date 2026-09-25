<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDimXpertSphereFeature~GetNominalSphere.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| GetNominalSphere Method (ISwDMDimXpertSphereFeature) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMDimXpertSphereFeature Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDimXpertSphereFeature.html) : GetNominalSphere Method (ISwDMDimXpertSphereFeature) |

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
:   x coordinate of the sphere origin

*Y*
:   y coordinate of the sphere origin

*Z*
:   z coordinate of the sphere origin

Gets the origin coordinates and radius of this DimXpert sphere.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetNominalSphere( _    ByRef R As System.Double, _    ByRef X As System.Double, _    ByRef Y As System.Double, _    ByRef Z As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMDimXpertSphereFeature Dim R As System.Double Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim value As System.Boolean   value = instance.GetNominalSphere(R, X, Y, Z) ``` | |

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
:   x coordinate of the sphere origin

*Y*
:   y coordinate of the sphere origin

*Z*
:   z coordinate of the sphere origin

#### Return Value

True if method call is successful; false otherwise

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMDimXpertSphereFeature::GetNominalSphere.

# ![](dotnetimages/collapse.gif)Example

See the examples on the interface page.

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMDimXpertSphereFeature Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDimXpertSphereFeature.html)

[ISwDMDimXpertSphereFeature Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDimXpertSphereFeature_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0