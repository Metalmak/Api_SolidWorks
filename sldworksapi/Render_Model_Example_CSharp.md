<!-- source: sldworksapi/Render_Model_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Render Model (C#)

This example shows how to use PhotoView 360 to render a model and save the
rendered image in BMP and HDR formats. You must have a SOLIDWORKS Premium
license to run this example.

//----------------------------------------------------------------------------
// Preconditions:
// 1. Verify that:
//    \* specified part exists.
//    \* **c:\temp** exists.
//    \* PhotoView 360 add-in is loaded in SOLIDWORKS.
// 2. Open the Immediate window.
//
// Postconditions:
// 1. If prompted to use perspective views in renderings, click
//    **Continue without Camera or Perspective**.
// 2. Changes the specified rendering options.
// 3. Creates **c:\temp\Filter\_1.bmp** and **c:\temp\Filter\_2.hdr**
containing
//    rendered images of the part.
// 4. Examine the Immediate window and **c:\temp**.
//
// NOTE: Rendering can take several minutes to complete.
//---------------------------------------------------------------------------
using Microsoft.VisualBasic;
using System;
using System.Collections;
using System.Collections.Generic;
using System.Data;
using System.Diagnostics;
using SolidWorks.Interop.sldworks;
using SolidWorks.Interop.swconst;
using System.Runtime.InteropServices;

namespace RayTraceRendererCSharp.csproj
{
    partial class SolidWorksMacro
    {

        ModelDoc2 swModel;
        RayTraceRenderer swRayTraceRenderer;
        RayTraceRendererOptions swRayTraceRenderOptions;
        int errors;
        int warnings;
        string fileName;

        bool status;

        public void Main()
        {
            fileName = "C:\\Users\\Public\\Documents\\SOLIDWORKS\\SOLIDWORKS
2018\\samples\\tutorial\\routing-pipes\\fittings\\filter.sldprt";
            swModel = swApp.**OpenDoc6**(fileName, (int)swDocumentTypes\_e.swDocPART, (int)swOpenDocOptions\_e.swOpenDocOptions\_Silent, "", ref errors, ref warnings);

            // Access PhotoView 360
            swRayTraceRenderer = (RayTraceRenderer)swApp.**GetRayTraceRenderer**((int)swRayTraceRenderType\_e.swPhotoView);

            // Get and set rendering options
            swRayTraceRenderOptions = swRayTraceRenderer.**RayTraceRendererOptions**;

            // Get current rendering values
            Debug.Print("Current rendering values");
            Debug.Print("  Image height = " + swRayTraceRenderOptions.**ImageHeight**);
            Debug.Print("  Image width = " + swRayTraceRenderOptions.**ImageWidth**);
            Debug.Print("  Image format = " + swRayTraceRenderOptions.**ImageFormat**);
            Debug.Print("  Preview render quality = " + swRayTraceRenderOptions.**PreviewRenderQuality**);
            Debug.Print("  Final render quality = " + swRayTraceRenderOptions.**FinalRenderQuality**);
            Debug.Print("  Bloom enabled? " + swRayTraceRenderOptions.**BloomEnabled**);
            Debug.Print("  Bloom threshold = " + swRayTraceRenderOptions.**BloomThreshold**);
            Debug.Print("  Bloom radius = " + swRayTraceRenderOptions.**BloomRadius**);
            Debug.Print("  Contour/cartoon
rendering enabled? " + swRayTraceRenderOptions.**ContourCartoonRenderingEnabled**);
            Debug.Print("
Render type = " + swRayTraceRenderOptions.**RenderType**);
            Debug.Print("  Shaded contour? " + swRayTraceRenderOptions.**ShadedContour**);
            Debug.Print("  Contour line thickness = " + swRayTraceRenderOptions.**ContourLineThickness**);
            Debug.Print("  Contour line color = " + swRayTraceRenderOptions.**ContourLineColor**);
            Debug.Print("  Use SOLIDWORKS view aspect ratio? " + swRayTraceRenderOptions.**UseSolidWorksViewAspectRatio**);

Debug.Print("  Alpha output?
" + swRayTraceRenderOptions.**AlphaOutput**);
            Debug.Print(" ");

            // Change rendering values
            Debug.Print("New rendering values");
            swRayTraceRenderOptions.**ImageHeight** = 567;
            Debug.Print("  Image height = " + swRayTraceRenderOptions.**ImageHeight**);
            swRayTraceRenderOptions.**ImageWidth** = 678;
            Debug.Print("  Image width = " + swRayTraceRenderOptions.**ImageWidth**);
            swRayTraceRenderOptions.**ImageFormat** = (int)swRayTraceRenderImageFormat\_e.swImageFormat\_HDR;
            Debug.Print("  Image format = " + swRayTraceRenderOptions.**ImageFormat**);
            swRayTraceRenderOptions.**PreviewRenderQuality** = (int)swRayTraceRenderQuality\_e.swRenderQuality\_Better;
            Debug.Print("  Preview render quality = " + swRayTraceRenderOptions.**PreviewRenderQuality**);
            swRayTraceRenderOptions.**FinalRenderQuality** = (int)swRayTraceRenderQuality\_e.swRenderQuality\_Best;
            Debug.Print("  Final render quality = " + swRayTraceRenderOptions.**FinalRenderQuality**);
            swRayTraceRenderOptions.**BloomEnabled** = false;
            Debug.Print("  Bloom enabled? " + swRayTraceRenderOptions.**BloomEnabled**);
            swRayTraceRenderOptions.**BloomThreshold** = 70;
            Debug.Print("  Bloom threshold = " + swRayTraceRenderOptions.**BloomThreshold**);
            swRayTraceRenderOptions.**BloomRadius** = 4;
            Debug.Print("  Bloom radius = " + swRayTraceRenderOptions.**BloomRadius**);
            swRayTraceRenderOptions.**ContourCartoonRenderingEnabled** = true;
            Debug.Print("  Contour/cartoon
rendering enabled? " + swRayTraceRenderOptions.**ContourCartoonRenderingEnabled**);
            swRayTraceRenderOptions.**RenderType** = (int)swRayTraceRenderingType\_e.swRayTraceContour;
            Debug.Print("  Render
type = " + swRayTraceRenderOptions.**RenderType);**
            swRayTraceRenderOptions.**ShadedContour** = false;
            Debug.Print("  Shaded contour? " + swRayTraceRenderOptions.**ShadedContour**);
            swRayTraceRenderOptions.**ContourLineThickness** = 3;
            Debug.Print("  Contour line thickness = " + swRayTraceRenderOptions.**ContourLineThickness**);
            swRayTraceRenderOptions.**ContourLineColor** = 255;
            Debug.Print("  Contour line color = " + swRayTraceRenderOptions.**ContourLineColor**);
            swRayTraceRenderOptions.**UseSolidWorksViewAspectRatio** = true;
            Debug.Print("  Use SOLIDWORKS view aspect ratio? " + swRayTraceRenderOptions.**UseSolidWorksViewAspectRatio**);

            // Display the preview window
            //status = swRayTraceRenderer.**DisplayPreviewWindow**
            // Display final render window
            //status = swRayTraceRenderer.**InvokeFinalRender**

            // Render in HDR format
            status = swRayTraceRenderer.**RenderToFile**("c:\\temp\\Filter\_2", 0, 0);
            // Render in BMP format
            swRayTraceRenderOptions.**ImageFormat** = (int)swRayTraceRenderImageFormat\_e.swImageFormat\_WindowsBmp;
            status = swRayTraceRenderer.**RenderToFile**("c:\\temp\\Filter\_1", 0, 0);

            // Abort final render
            //status = swRayTraceRenderer.**AbortFinalRender**
// Close preview and final render windows
            //status = swRayTraceRenderer.**CloseRayTraceRender**

        }

        public SldWorks swApp;

    }

}