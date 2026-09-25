<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~ReverseEvaluate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ReverseEvaluate Method (ICurve) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html) : ReverseEvaluate Method (ICurve) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PositionX*
:   X coordinate of this location on the curve

*PositionY*
:   Y coordinate of this location on the curve

*PositionZ*
:   Z coordinate of this location on the curve

Gets the U parameter for the given XYZ location on this curve.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ReverseEvaluate( _    ByVal PositionX As System.Double, _    ByVal PositionY As System.Double, _    ByVal PositionZ As System.Double _ ) As System.Double ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICurve Dim PositionX As System.Double Dim PositionY As System.Double Dim PositionZ As System.Double Dim value As System.Double   value = instance.ReverseEvaluate(PositionX, PositionY, PositionZ) ``` | |

| C# |  |
| --- | --- |
| ``` System.double ReverseEvaluate(     System.double PositionX,    System.double PositionY,    System.double PositionZ ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.double ReverseEvaluate(  &   System.double PositionX, &   System.double PositionY, &   System.double PositionZ ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PositionX*
:   X coordinate of this location on the curve

*PositionY*
:   Y coordinate of this location on the curve

*PositionZ*
:   Z coordinate of this location on the curve

#### Return Value

U parameter value for this location on the curve

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Curve::ReverseEvaluate.

# ![](dotnetimages/collapse.gif)Example

[Get UV Parameters for XYZ Location (VBA)](Get_UV_Parameters_For_XYZ_Location_Example_VB.htm)

[Get UV Parameters for XYZ Location (VB.NET)](Get_UV_Parameters_For_XYZ_Location_Example_VBNET.htm)

[Get UV Parameters for XYZ Location (C#)](Get_UV_Parameters_For_XYZ_Location_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[ICurve Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve.html)

[ICurve Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve_members.html)

[IFace2::ReverseEvaluate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2~ReverseEvaluate.html)

[IFace2::IReverseEvaluate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2~IReverseEvaluate.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0