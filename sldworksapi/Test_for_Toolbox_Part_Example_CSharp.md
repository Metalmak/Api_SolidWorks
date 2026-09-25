<!-- source: sldworksapi/Test_for_Toolbox_Part_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Test for Toolbox Part Example (C#)

This example shows how to test whether a part is a Toolbox part.

//----------------------------------------------------------------------------
// Preconditions: Open *public\_documents***\samples\tutorial\api\bagel.sldprt**.
//
// Postconditions: Inspect the Immediate window for the Toolbox part type.
//
// NOTE: Because the model is used elsewhere,
// do not save changes when closing it.
//
---------------------------------------------------------------------------
using
SolidWorks.Interop.sldworks;
using
SolidWorks.Interop.swconst;
using
System.Runtime.InteropServices;
using
System;
using
System.Diagnostics;
namespace
ToolboxPartType\_CSharp.csproj
{
    partial
class
SolidWorksMacro
    {

        ModelDoc2
part;
        ModelDocExtension
modelDocExt;

        int
ret;

        public
void Main()
        {
            part = (ModelDoc2)swApp.**ActiveDoc**;
            modelDocExt = part.**Extension**;
            ret = modelDocExt.**ToolboxPartType**;

            Debug.Print("Toolbox
part type as defined in swToolBoxPartType\_e? "
+ ret);

        }

        public
SldWorks
swApp;

    }
}