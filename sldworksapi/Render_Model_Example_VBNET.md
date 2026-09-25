<!-- source: sldworksapi/Render_Model_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Render Model (VB.NET)

This example shows how to use PhotoView 360 to render a model and save the
rendered image in BMP and HDR formats. You must have a SOLIDWORKS Premium
license to run this example.

'----------------------------------------------------------------------------
' Preconditions:
' 1. Verify that:
'    \* specified part exists.
'    \* **c:\temp** exists.
'    \* PhotoView 360 add-in is loaded in SOLIDWORKS.
' 2. Open the Immediate window.
'
' Postconditions:
' 1. If prompted to use perspective views in renderings, click
'    **Continue without Camera or Perspective**.
' 2. Changes the specified rendering options.
' 3. Creates **c:\temp\Filter\_1.bmp** and **c:\temp\Filter\_2.hdr**
containing
'    rendered images of the part.
' 4. Examine the Immediate window and **c:\temp**.
'
' NOTE: Rendering can take several minutes to complete.
'---------------------------------------------------------------------------