<!-- source: swdocmgrapi/SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDimXpertCompoundClosedSlot3dFeature~GetNominalClosedSlot.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Document Manager API Help | Send comments on this topic. |
| GetNominalClosedSlot Method (ISwDMDimXpertCompoundClosedSlot3dFeature) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdocumentmgr Namespace](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr_namespace.html) > [ISwDMDimXpertCompoundClosedSlot3dFeature Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDimXpertCompoundClosedSlot3dFeature.html) : GetNominalClosedSlot Method (ISwDMDimXpertCompoundClosedSlot3dFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*width*
:   Width of the compound closed slot

*Length*
:   Length of the compound closed slot

*X*
:   x coordinate of the compound closed slot

*Y*
:   y coordinate of the compound closed slot

*Z*
:   z coordinate of the compound closed slot

*I*
:   i component of the direction vector of the compound closed slot

*J*
:   j component of the direction vector of the compound closed slot

*K*
:   k component of the direction vector of the compound closed slot

*LongitudeI*
:   i component of the longitudinal unit vector of the closed slot

*LongitudeJ*
:   j component of the longitudinal unit vector of the closed slot

*LongitudeK*
:   k component of the longitudinal unit vector of the closed slot

Gets various attributes for this DimXpert compound closed slot.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetNominalClosedSlot( _    ByRef width As System.Double, _    ByRef Length As System.Double, _    ByRef X As System.Double, _    ByRef Y As System.Double, _    ByRef Z As System.Double, _    ByRef I As System.Double, _    ByRef J As System.Double, _    ByRef K As System.Double, _    ByRef LongitudeI As System.Double, _    ByRef LongitudeJ As System.Double, _    ByRef LongitudeK As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISwDMDimXpertCompoundClosedSlot3dFeature Dim width As System.Double Dim Length As System.Double Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim I As System.Double Dim J As System.Double Dim K As System.Double Dim LongitudeI As System.Double Dim LongitudeJ As System.Double Dim LongitudeK As System.Double Dim value As System.Boolean   value = instance.GetNominalClosedSlot(width, Length, X, Y, Z, I, J, K, LongitudeI, LongitudeJ, LongitudeK) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetNominalClosedSlot(     out System.double width,    out System.double Length,    out System.double X,    out System.double Y,    out System.double Z,    out System.double I,    out System.double J,    out System.double K,    out System.double LongitudeI,    out System.double LongitudeJ,    out System.double LongitudeK ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetNominalClosedSlot(  &   [Out] System.double width, &   [Out] System.double Length, &   [Out] System.double X, &   [Out] System.double Y, &   [Out] System.double Z, &   [Out] System.double I, &   [Out] System.double J, &   [Out] System.double K, &   [Out] System.double LongitudeI, &   [Out] System.double LongitudeJ, &   [Out] System.double LongitudeK ) ``` | |

#### Parameters

*width*
:   Width of the compound closed slot

*Length*
:   Length of the compound closed slot

*X*
:   x coordinate of the compound closed slot

*Y*
:   y coordinate of the compound closed slot

*Z*
:   z coordinate of the compound closed slot

*I*
:   i component of the direction vector of the compound closed slot

*J*
:   j component of the direction vector of the compound closed slot

*K*
:   k component of the direction vector of the compound closed slot

*LongitudeI*
:   i component of the longitudinal unit vector of the closed slot

*LongitudeJ*
:   j component of the longitudinal unit vector of the closed slot

*LongitudeK*
:   k component of the longitudinal unit vector of the closed slot

#### Return Value

True if method call is successful; false otherwise

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SwDMDimXpertCompoundClosedSlot3dFeature::GetNominalClosedSlot.

# ![](dotnetimages/collapse.gif)Example

See the examples on the interface page.

# ![](dotnetimages/collapse.gif)Remarks

The i, j, and k components of the longitudinal vector indicate the direction of a feature's length with respect to its part axes. For example, if the length of a feature goes along the y-axis of the part, its longitudinal vector is (0, 1, 0).

# ![](dotnetimages/collapse.gif)See Also

####

[ISwDMDimXpertCompoundClosedSlot3dFeature Interface](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDimXpertCompoundClosedSlot3dFeature.html)

[ISwDMDimXpertCompoundClosedSlot3dFeature Members](SolidWorks.Interop.swdocumentmgr~SolidWorks.Interop.swdocumentmgr.ISwDMDimXpertCompoundClosedSlot3dFeature_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0