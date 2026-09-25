<!-- source: sldworksapi/Flip_Sketch_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Flip Sketch Example (C#)

This example shows how to flip a sketch about a coordinate system axis.

//-------------------------------------------------------------------------
// Preconditions: Open a model document and select a sketch.
//
// Postconditions: Flips the sketch about the x axis.
//------------------------------------------------------------------------
using
Microsoft.VisualBasic;
using
System;
using
System.Collections;
using
System.Collections.Generic;
using
System.Data;
using
System.Diagnostics;
using
SolidWorks.Interop.sldworks;
using
SolidWorks.Interop.swconst;
using
System.Runtime.InteropServices;
namespace
FlipSketch\_CSharp.csproj
{
    partial
class
SolidWorksMacro
    {
        public
void Main()
        {
            ModelDoc2
swModel = default(ModelDoc2);
            swModel = (ModelDoc2)swApp.**ActiveDoc**;

            swModel.**SketchModifyFlip**(1);

        }

        public
SldWorks
swApp;
    }
}