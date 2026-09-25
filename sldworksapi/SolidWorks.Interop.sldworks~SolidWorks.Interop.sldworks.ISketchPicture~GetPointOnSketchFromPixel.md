<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture~GetPointOnSketchFromPixel.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetPointOnSketchFromPixel Method (ISketchPicture) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchPicture Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture.html) : GetPointOnSketchFromPixel Method (ISketchPicture) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Row*
:   Row for this pixel

*Column*
:   Column for this pixel

Gets the sketch coordinate for the specified pixel.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetPointOnSketchFromPixel( _    ByVal Row As System.Integer, _    ByVal Column As System.Integer _ ) As MathPoint ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchPicture Dim Row As System.Integer Dim Column As System.Integer Dim value As MathPoint   value = instance.GetPointOnSketchFromPixel(Row, Column) ``` | |

| C# |  |
| --- | --- |
| ``` MathPoint GetPointOnSketchFromPixel(     System.int Row,    System.int Column ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` MathPoint^ GetPointOnSketchFromPixel(  &   System.int Row, &   System.int Column ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Row*
:   Row for this pixel

*Column*
:   Column for this pixel

#### Return Value

[Point](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IMathPoint.html) in the sketch space

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchPicture::GetPointOnSketchFromPixel.

# ![](dotnetimages/collapse.gif)Remarks

This method gets a point in the sketch space for the specified 0-based row and column indices from the pixel map. Because the bitmap data is raw data, this method helps determine where a point on the sketch is for the pixel after all of the transformation information has been applied. This method helps connect the raw data to its sketch.

See [ISketchPicture::GetPixelmap](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchPicture~GetPixelmap.html) or [ISketchPicture::IGetPixelmap](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchPicture~IGetPixelmap.html) for more information about the pixel map.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchPicture Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture.html)

[ISketchPicture Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture_members.html)

[ISketchPicture::GetPixelmapSize Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture~GetPixelmapSize.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0