<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRayTraceRenderer~RenderToFile.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| RenderToFile Method (IRayTraceRenderer) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IRayTraceRenderer Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRayTraceRenderer.html) : RenderToFile Method (IRayTraceRenderer) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ImageFileName*
:   File path and name (see **Remarks**)

*Width*
:   Width of image in pixels (see **Remarks**)

*Height*
:   Height of image in pixels (see **Remarks**)

Saves the current view of the rendered model as an image to the specified file.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function RenderToFile( _    ByVal ImageFileName As System.String, _    ByVal Width As System.Integer, _    ByVal Height As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IRayTraceRenderer Dim ImageFileName As System.String Dim Width As System.Integer Dim Height As System.Integer Dim value As System.Boolean   value = instance.RenderToFile(ImageFileName, Width, Height) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool RenderToFile(     System.string ImageFileName,    System.int Width,    System.int Height ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool RenderToFile(  &   System.String^ ImageFileName, &   System.int Width, &   System.int Height ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ImageFileName*
:   File path and name (see **Remarks**)

*Width*
:   Width of image in pixels (see **Remarks**)

*Height*
:   Height of image in pixels (see **Remarks**)

#### Return Value

True if the current view of the rendered model is saved, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See RayTraceRenderer::RenderToFile.

# ![](dotnetimages/collapse.gif)Example

[Render Model (C#)](Render_Model_Example_CSharp.htm)

[Render Model (VB.NET)](Render_Model_Example_VBNET.htm)

[Render Model (VBA)](Render_Model_Example_VB.htm)

[Include Note in Render File (C#)](Include_Note_in_Render_File_Example_CSharp.htm)

[Include Note in Render File (VB.NET)](Include_Note_in_Render_File_Example_VBNET.htm)

[Include Note in Render File (VBA)](Include_Note_in_Render_File_Example_VB.htm)

# ![](dotnetimages/collapse.gif)Remarks

Before calling this method:

* you can call [IRayTraceRendererOptions::ImageFormat](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRayTraceRendererOptions~ImageFormat.html) to specify the image format in which to save the model and omit the file format extension when specifying ImageFileName.* set [IRayTraceRendererOptions::IncludeAnnotationsInRendering](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRayTraceRendererOptions~IncludeAnnotationsInRendering.html) to true to include annotations and dimensions visible in the model in the render file. You can also set [IRayTraceRendererOptions::RenderAnnotationsToSeparateImage](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRayTraceRendererOptions~RenderAnnotationsToSeparateImage.html) to true to render the annotations and dimensions visible in the model to a separate image file.

You can override the values set in [IRayTraceRendererOptions::ImageWidth](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRayTraceRendererOptions~ImageWidth.html) and [IRayTraceRendererOptions::ImageHeight](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IRayTraceRendererOptions~ImageHeight.html) by calling this method with specific values for Width and Height. Set Width and Height to 0 to use values specified by IRayTraceRendererOptions::ImageWidth and IRayTraceRendererOptions::ImageHeight.

After calling this method, call [IRayTraceRenderer::CloseRayTraceRender](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRayTraceRenderer~CloseRayTraceRender.html).

# ![](dotnetimages/collapse.gif)See Also

####

[IRayTraceRenderer Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRayTraceRenderer.html)

[IRayTraceRenderer Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRayTraceRenderer_members.html)

[IRayTraceRenderer::InvokeFinalRender Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRayTraceRenderer~InvokeFinalRender.html)

[IRayTraceRendererOptions::UpdateGraphics Method ()](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IRayTraceRendererOptions~UpdateGraphics.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0