<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager~InsertSketchPicture2.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertSketchPicture2 Method (ISketchManager) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html) : InsertSketchPicture2 Method (ISketchManager) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Path to image file including file extension

*HighestResolution*
:   True to insert images up to 8192 pixels without compression, false to compress images to 2048 pixels before insertion (see **Remarks**)

Inserts a picture on the current drawing sketch.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertSketchPicture2( _    ByVal FileName As System.String, _    ByVal HighestResolution As System.Boolean _ ) As SketchPicture ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISketchManager Dim FileName As System.String Dim HighestResolution As System.Boolean Dim value As SketchPicture   value = instance.InsertSketchPicture2(FileName, HighestResolution) ``` | |

| C# |  |
| --- | --- |
| ``` SketchPicture InsertSketchPicture2(     System.string FileName,    System.bool HighestResolution ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` SketchPicture^ InsertSketchPicture2(  &   System.String^ FileName, &   System.bool HighestResolution ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*
:   Path to image file including file extension

*HighestResolution*
:   True to insert images up to 8192 pixels without compression, false to compress images to 2048 pixels before insertion (see **Remarks**)

#### Return Value

[Picture](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISketchPicture.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SketchManager::InsertSketchPicture2.

# ![](dotnetimages/collapse.gif)Example

[Flip Sketch Picture (VBA)](Flip_Sketch_Picture_Example_VB.htm)

[Flip Sketch Picture (VB.NET)](Flip_Sketch_Picture_Example_VBNET.htm)

[Flip Sketch Picture (C#)](Flip_Sketch_Picture_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

If the document type is not a drawing, then HighestResolution defaults to false.

# ![](dotnetimages/collapse.gif)See Also

####

[ISketchManager Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager.html)

[ISketchManager Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISketchManager_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 SP04, Revision Number 27.4