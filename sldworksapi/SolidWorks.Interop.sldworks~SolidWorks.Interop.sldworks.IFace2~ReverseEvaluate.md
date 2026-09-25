<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2~ReverseEvaluate.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| ReverseEvaluate Method (IFace2) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFace2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html) : ReverseEvaluate Method (IFace2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*PositionX*
:   X coordinate of this location on the face

*PositionY*
:   Y coordinate of this location on the face

*PositionZ*
:   Z coordinate of this location on the face

Gets the UV parameters for the given XYZ location on this face.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function ReverseEvaluate( _    ByVal PositionX As System.Double, _    ByVal PositionY As System.Double, _    ByVal PositionZ As System.Double _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFace2 Dim PositionX As System.Double Dim PositionY As System.Double Dim PositionZ As System.Double Dim value As System.Object   value = instance.ReverseEvaluate(PositionX, PositionY, PositionZ) ``` | |

| C# |  |
| --- | --- |
| ``` System.object ReverseEvaluate(     System.double PositionX,    System.double PositionY,    System.double PositionZ ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ ReverseEvaluate(  &   System.double PositionX, &   System.double PositionY, &   System.double PositionZ ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*PositionX*
:   X coordinate of this location on the face

*PositionY*
:   Y coordinate of this location on the face

*PositionZ*
:   Z coordinate of this location on the face

#### Return Value

Array of two doubles representing the U and V parameters of this location on the face

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Face2::ReverseEvaluate.

# ![](dotnetimages/collapse.gif)Example

[Get UV Parameters for XYZ Location (VBA)](Get_UV_Parameters_For_XYZ_Location_Example_VB.htm)

[Get UV Parameters for XYZ Location (VB.NET)](Get_UV_Parameters_For_XYZ_Location_Example_VBNET.htm)

[Get UV Parameters for XYZ Location (C#)](Get_UV_Parameters_For_XYZ_Location_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

This method returns corrected UV parameters for periodic surfaces; thus, you should use this method when dealing with periodic surfaces.

For example, you can have a cylindrical surface that extends from 0 to 2pi in the Udir. The face related to this surface in some cases extends from 0 to pi, then from 0 to pi again. In this case, neither [ISurface::IReverseEvaluate](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface~IReverseEvaluate.html) nor [ISurface::ReverseEvaluate](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISurface~ReverseEvaluate.html) will work for values greater than pi (the returned U value will be greater than Maximum U for the face). However, [IFace2::IReverseEvaluate](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFace2~IReverseEvaluate.html), and IFace2::ReverseEvaluate, will return the correct values.

# ![](dotnetimages/collapse.gif)See Also

####

[IFace2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2.html)

[IFace2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFace2_members.html)

[ICurve::ReverseEvaluate Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICurve~ReverseEvaluate.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2010 FCS, Revision Number 18.0