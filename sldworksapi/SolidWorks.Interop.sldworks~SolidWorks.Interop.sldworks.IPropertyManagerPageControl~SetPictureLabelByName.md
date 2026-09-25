<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageControl~SetPictureLabelByName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetPictureLabelByName Method (IPropertyManagerPageControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPropertyManagerPageControl Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageControl.html) : SetPictureLabelByName Method (IPropertyManagerPageControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ColorBitmap*
:   Fully qualified path to the location of the bitmap (i.e., the graphic to use) on disk

*MaskBitmap*
:   Fully qualified path to the location of the alpha mask bitmap on disk

Sets the bitmap label for this control on a PropertyManager page.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetPictureLabelByName( _    ByVal ColorBitmap As System.String, _    ByVal MaskBitmap As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPropertyManagerPageControl Dim ColorBitmap As System.String Dim MaskBitmap As System.String Dim value As System.Boolean   value = instance.SetPictureLabelByName(ColorBitmap, MaskBitmap) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetPictureLabelByName(     System.string ColorBitmap,    System.string MaskBitmap ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetPictureLabelByName(  &   System.String^ ColorBitmap, &   System.String^ MaskBitmap ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ColorBitmap*
:   Fully qualified path to the location of the bitmap (i.e., the graphic to use) on disk

*MaskBitmap*
:   Fully qualified path to the location of the alpha mask bitmap on disk

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PropertyManagerPageControl::SetPictureLabelByName.

# ![](dotnetimages/collapse.gif)Remarks

The image format for the two bitmaps is 18 x 18 pixels x 256 colors. The pixels in MaskBitmap specify transparency through shades of grey with boundaries of black pixels = 100% opaque and white pixels = 100% transparent.

You can only use this method on a PropertyManager page before the page is displayed, while it is displayed, or when it is closed.

# ![](dotnetimages/collapse.gif)See Also

####

[IPropertyManagerPageControl Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageControl.html)

[IPropertyManagerPageControl Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPropertyManagerPageControl_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0