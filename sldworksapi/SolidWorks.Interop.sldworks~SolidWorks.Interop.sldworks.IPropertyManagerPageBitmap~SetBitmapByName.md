<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageBitmap~SetBitmapByName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetBitmapByName Method (IPropertyManagerPageBitmap) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPageBitmap Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageBitmap.html) : SetBitmapByName Method (IPropertyManagerPageBitmap) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ColorBitmap*
:   Full path and filename of the bitmap on disk

*MaskBitmap*
:   Full path and filename of the alpha mask bitmap on disk

Sets the bitmap for this control.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetBitmapByName( _    ByVal ColorBitmap As System.String, _    ByVal MaskBitmap As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageBitmap Dim ColorBitmap As System.String Dim MaskBitmap As System.String Dim value As System.Boolean   value = instance.SetBitmapByName(ColorBitmap, MaskBitmap) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetBitmapByName(     System.string ColorBitmap,    System.string MaskBitmap ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetBitmapByName(  &   System.String^ ColorBitmap, &   System.String^ MaskBitmap ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ColorBitmap*
:   Full path and filename of the bitmap on disk

*MaskBitmap*
:   Full path and filename of the alpha mask bitmap on disk

#### Return Value

True if the bitmap is set for this control, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageBitmap::SetBitmapByName.

# ![](dotnetimages/collapse.gif)Remarks

If you are creating a PropertyManager page add-in and ColorBitmap is either invalid or has the wrong path, this method displays an alternative image and returns false.

The typical image format for the two SOLIDWORKS bitmaps is 18 x 18 pixels x 256 colors. Using this method, you can specify a bigger bitmap, e.g., 24 x 24 pixels, to get extra detail. The pixels in MaskBitmap specify transparency through shades of grey with boundaries of black pixels = 100% opaque and white pixels = 100% transparent.

Use [IPropertyManagerPageControl::Top](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPageControl~Top.html) to set the top of the control and use [IPropertyManagerPageControl::Tip](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPropertyManagerPageControl~Tip.html) to set the ToolTip.

You can use this method before, during, or after the PropertyManager page is displayed or closed. If you use this method when the PropertyManager page is displayed, use bitmaps that are the same size.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageBitmap Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageBitmap.html)

[IPropertyManagerPageBitmap Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageBitmap_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 FCS, Revision Number 15.0