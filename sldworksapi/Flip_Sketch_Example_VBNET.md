<!-- source: sldworksapi/Flip_Sketch_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Flip Sketch Example (VB.NET)

This example shows how to flip a sketch about a coordinate system axis.

'-------------------------------------------------------------------------
' Preconditions: Open a model document and select a sketch.
'
' Postconditions: Flips the sketch about the x axis.
'------------------------------------------------------------------------
Imports
SolidWorks.Interop.sldworks
Imports
SolidWorks.Interop.swconst
Imports
System.Runtime.InteropServices
Imports
System

Partial
Class
SolidWorksMacro

    Sub
main()

        Dim
swModel As
ModelDoc2
        swModel = swApp.**ActiveDoc**

        swModel.**SketchModifyFlip**(1)

    End
Sub

    Public
swApp As
SldWorks

End
Class