<!-- source: sldworksapi/Rebuild_an_Assembly_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Rebuild an Assembly Example (C#)

This example shows how to rebuild an assembly.

//----------------------------------------------------------------------------
// Preconditions: Open *public\_documents***\samples\tutorial\api\wrench.sldasm**.
//
// Postconditions:
// 1. Rebuilds the assembly.
// 2. Inspect the Immediate window for the result code.
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
Rebuild\_CSharp.csproj
{
    partial
class
SolidWorksMacro
    {

        ModelDoc2
part;
        ModelDocExtension
modelDocExt;

        bool
ret;

        public
void Main()
        {
            part = (ModelDoc2)swApp.**ActiveDoc**;
            modelDocExt = part.**Extension**;
            ret = modelDocExt.**Rebuild**((int)swRebuildOptions\_e.swRebuildAll);

            Debug.Print("Successfully
rebuilt? " + ret);

        }

        public
SldWorks
swApp;

    }

}