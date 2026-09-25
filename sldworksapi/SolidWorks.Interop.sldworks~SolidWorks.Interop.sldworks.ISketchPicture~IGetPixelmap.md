<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture~IGetPixelmap.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IGetPixelmap Method (ISketchPicture) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchPicture Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture.html) : IGetPixelmap Method (ISketchPicture) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Count*
:   Size of the array

Gets the picture pixels.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function IGetPixelmap( _    ByVal Count As System.Integer _ ) As System.Short ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchPicture Dim Count As System.Integer Dim value As System.Short   value = instance.IGetPixelmap(Count) ``` | |

| C# |  |
| --- | --- |
| ``` System.short IGetPixelmap(     System.int Count ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.short IGetPixelmap(  &   System.int Count ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Count*
:   Size of the array

#### Return Value

* in-process, unmanaged C++: Pointer to an array containing groups of 3 or 4 values (see **Remarks**)

- VBA, VB.NET, C#, and C++/CLI: Not supported

  See In-process Methods for details about this type of method.

# ![](dotnetimages/collapse.gif)Remarks

The array contains groups of three, the Red, Green, Blue (RGB) components of pixel color, and optionally, a fourth value that indicates the transparency of the pixel, which can be a value from 0 (transparent) to 255 (opaque).

Before calling this method, call [ISketchPicture::GetPixelmapSize](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchPicture~GetPixelmapSize.html) to get the value of Count.

To determine the format of the data, you need the information returned by ISketchPicture::GetPixelmapSize:

Number of items per pixel = size / (rows \* columns)

Each group of three or four goes across each pixel in a row of the bitmap. The next row follows in the array.

This raw data does not include translation, scaling, rotation, and flipping. SOLIDWORKS applies these properties to the raw bitmap data to draw it in the sketch.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchPicture Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture.html)

[ISketchPicture Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture_members.html)

[ISketchPicture::GetPixelmap Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture~GetPixelmap.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0