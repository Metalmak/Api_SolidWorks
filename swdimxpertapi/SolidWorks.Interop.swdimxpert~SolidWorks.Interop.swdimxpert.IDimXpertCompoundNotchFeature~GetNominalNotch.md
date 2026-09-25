<!-- source: swdimxpertapi/SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertCompoundNotchFeature~GetNominalNotch.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS DimXpert API Help | Send comments on this topic. |
| GetNominalNotch Method (IDimXpertCompoundNotchFeature) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.swdimxpert Namespace](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert_namespace.html) > [IDimXpertCompoundNotchFeature Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertCompoundNotchFeature.html) : GetNominalNotch Method (IDimXpertCompoundNotchFeature) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Width*
:   Width of the notch

*Length*
:   Length of the notch

*X*
:   X-coordinate of the notch

*Y*
:   Y-coordinate of the notch

*Z*
:   Z-coordinate of the notch

*I*
:   I component of the direction vector of the notch

*J*
:   J component of the direction vector of the notch

*K*
:   K component of the direction vector of the notch

*LongitudeI*
:   I component of the longitudinal unit vector of the notch

*LongitudeJ*
:   J component of the longitudinal unit vector of the notch

*LongitudeK*
:   K component of the longitudinal unit vector of the notch

Gets various attributes for this DimXpert compound notch.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetNominalNotch( _    ByRef Width As System.Double, _    ByRef Length As System.Double, _    ByRef X As System.Double, _    ByRef Y As System.Double, _    ByRef Z As System.Double, _    ByRef I As System.Double, _    ByRef J As System.Double, _    ByRef K As System.Double, _    ByRef LongitudeI As System.Double, _    ByRef LongitudeJ As System.Double, _    ByRef LongitudeK As System.Double _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IDimXpertCompoundNotchFeature Dim Width As System.Double Dim Length As System.Double Dim X As System.Double Dim Y As System.Double Dim Z As System.Double Dim I As System.Double Dim J As System.Double Dim K As System.Double Dim LongitudeI As System.Double Dim LongitudeJ As System.Double Dim LongitudeK As System.Double Dim value As System.Boolean   value = instance.GetNominalNotch(Width, Length, X, Y, Z, I, J, K, LongitudeI, LongitudeJ, LongitudeK) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool GetNominalNotch(     out System.double Width,    out System.double Length,    out System.double X,    out System.double Y,    out System.double Z,    out System.double I,    out System.double J,    out System.double K,    out System.double LongitudeI,    out System.double LongitudeJ,    out System.double LongitudeK ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool GetNominalNotch(  &   [Out] System.double Width, &   [Out] System.double Length, &   [Out] System.double X, &   [Out] System.double Y, &   [Out] System.double Z, &   [Out] System.double I, &   [Out] System.double J, &   [Out] System.double K, &   [Out] System.double LongitudeI, &   [Out] System.double LongitudeJ, &   [Out] System.double LongitudeK ) ``` | |

#### Parameters

*Width*
:   Width of the notch

*Length*
:   Length of the notch

*X*
:   X-coordinate of the notch

*Y*
:   Y-coordinate of the notch

*Z*
:   Z-coordinate of the notch

*I*
:   I component of the direction vector of the notch

*J*
:   J component of the direction vector of the notch

*K*
:   K component of the direction vector of the notch

*LongitudeI*
:   I component of the longitudinal unit vector of the notch

*LongitudeJ*
:   J component of the longitudinal unit vector of the notch

*LongitudeK*
:   K component of the longitudinal unit vector of the notch

#### Return Value

True if method call is successful; false otherwise

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See DimXpertCompoundNotchFeature::GetNominalNotch.

# ![](dotnetimages/collapse.gif)Example

[Get More DimXpert Feature Examples (VBA)](Get_DimXpert_Feature2_Example_VB.htm)

[Get More DimXpert Feature Examples (VB.NET)](Get_DimXpert_Feature2_Example_VBNET.htm)

# ![](dotnetimages/collapse.gif)Remarks

The longitudinal i, j, and k component vectors indicate the direction of a notch's length with respect to its part axes. For example, if the length of a notch goes along the y-axis of the part, its longitudinal vector is (0, 1, 0).

# ![](dotnetimages/collapse.gif)See Also

####

[IDimXpertCompoundNotchFeature Interface](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertCompoundNotchFeature.html)

[IDimXpertCompoundNotchFeature Members](SolidWorks.Interop.swdimxpert~SolidWorks.Interop.swdimxpert.IDimXpertCompoundNotchFeature_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0