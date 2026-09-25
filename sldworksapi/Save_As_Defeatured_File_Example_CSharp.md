<!-- source: sldworksapi/Save_As_Defeatured_File_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Save as De-Featured File Example (C#)

This example shows how to de-feature an assembly and save it as a part.

//-----------------------------------------------------------------------------
// Preconditions:
// 1. Open public\_documents\samples\tutorial\floxpress\ball valve\ball\_valve.sldasm.
// 2. Verify that **c:\temp** exists.
//
// Postconditions:
// 1. Saves the assembly as a de-featured part.
// 2. Open **c:\temp\ball\_valve.sldprt** to verify.
//------------------------------------------------------------------------------
using SolidWorks.Interop.sldworks;
using SolidWorks.Interop.swconst;
using System;

namespace SaveFileAsDeFeaturedPart\_CSharp.csproj

{

    partial
class SolidWorksMacro

    {

        ModelDoc2
swModel;
        bool
boolstatus;

        public
void Main()
        {

            swModel= (ModelDoc2)swApp.**ActiveDoc**;
            boolstatus
= swModel.**Extension**.SaveDeFeaturedFile("C:\\temp\\ball\_valve.sldprt");

        }

        public
SldWorks swApp;

    }

}