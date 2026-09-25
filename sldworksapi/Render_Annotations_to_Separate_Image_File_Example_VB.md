<!-- source: sldworksapi/Render_Annotations_to_Separate_Image_File_Example_VB.htm -->

# SOLIDWORKS API Help

# Render Annotations to Separate Image File Example (VBA)

This example shows how to render annotations and dimensions visible in a
model to a separate image file.

```
'--------------------------------------------------------------
' Preconditions:
' 1. Open a model document.
' 2. Add a note to the model.
' 3. Right-click Annotations in the FeatureManager design tree
'    and click Show Feature Dimensions, if dimensions
'    are not visible in the model.
' 4. Verify that:
'    * PhotoView 360 add-in is loaded.
'    * c:\temp exists.
'
' Preconditions:
' 1. Sets the options to include and render annotations and dimensions
'    visible in a model to a separate image file.
' 2. If prompted to add camera or perspective, click Continue
'    without Camera or Perspective.
' 3. Renders:
'    * model to c:\temp\annotations.png
'    * note and dimensions to c:\temp\annotations_1.png
' 4. Open both files to verify the previous step.
'--------------------------------------------------------------
Option Explicit

Sub main()

        Dim swApp As SldWorks.SldWorks
        Dim swModel As SldWorks.ModelDoc2
        Dim swRayTraceRenderer As SldWorks.RayTraceRenderer
        Dim swRayTraceRenderOptions As SldWorks.RayTraceRendererOptions
        Dim status As Boolean

        Set swApp = Application.SldWorks
        Set swModel = swApp.ActiveDoc
```

```
        'Access PhotoView 360
        Set swRayTraceRenderer = swApp.GetRayTraceRenderer(swRayTraceRenderType_e.swPhotoView)
```

```
        'Set options to include and render annotations and dimensions
	'visible in a model to a separate image file
        Set swRayTraceRenderOptions = swRayTraceRenderer.RayTraceRendererOptions
	swRayTraceRenderOptions.IncludeAnnotationsInRendering = True
        swRayTraceRenderOptions.RenderAnnotationsToSeparateImage = True
        status = swRayTraceRenderer.RenderToFile("c:\temp\annotations.png", 0, 0)
        status = swRayTraceRenderer.CloseFinalRenderWindow

End Sub
```