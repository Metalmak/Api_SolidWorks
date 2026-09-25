<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture~SetSize.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetSize Method (ISketchPicture) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchPicture Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture.html) : SetSize Method (ISketchPicture) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Width*
:   Width of the picture in meters

*Height*
:   Height of the picture in meters

*AspectRatioLocked*
:   True to keep a fixed width and height aspect ratio, false to not

Sets the size of the picture on the sketch.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetSize( _    ByVal Width As System.Double, _    ByVal Height As System.Double, _    ByVal AspectRatioLocked As System.Boolean _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchPicture Dim Width As System.Double Dim Height As System.Double Dim AspectRatioLocked As System.Boolean Dim value As System.Boolean   value = instance.SetSize(Width, Height, AspectRatioLocked) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetSize(     System.double Width,    System.double Height,    System.bool AspectRatioLocked ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetSize(  &   System.double Width, &   System.double Height, &   System.bool AspectRatioLocked ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Width*
:   Width of the picture in meters

*Height*
:   Height of the picture in meters

*AspectRatioLocked*
:   True to keep a fixed width and height aspect ratio, false to not

#### Return Value

True if the size of the picture is set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchPicture::SetSize.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchPicture Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture.html)

[ISketchPicture Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture_members.html)

[ISketchPicture::GetSize Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchPicture~GetSize.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0