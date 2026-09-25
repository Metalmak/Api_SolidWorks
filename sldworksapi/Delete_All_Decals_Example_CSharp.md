<!-- source: sldworksapi/Delete_All_Decals_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Delete All Decals Example (C#)

This example shows how to delete all decals in a model.

//---------------------------------------------------------------------------

// Preconditions: Open a part with one or more decals.
//
// Postconditions: Deletes all of the decals from the
part.
//
--------------------------------------------------------------------------

using
SolidWorks.Interop.sldworks;
using
SolidWorks.Interop.swconst;
using
System.Runtime.InteropServices;
using
System;

namespace
DeleteAllDecals\_CSharp.csproj
{
    public
partial
class
SolidWorksMacro
    {

        public
void Main()
        {
            ModelDoc2
swModel;
            ModelDocExtension
swModelDocExt;
            Boolean
boolStatus;

            swModel = (ModelDoc2)swApp.**ActiveDoc**;
            swModelDocExt = (ModelDocExtension)swModel.**Extension**;
            boolStatus = swModelDocExt.**DeleteAllDecals**();

        }

        public
SldWorks
swApp;
    }
}