<!-- source: sldworksapi/Get_General_Table_in_Part_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Get General Table Annotation Example (C#)

This example shows how to create a general table annotation for 3D PDF files
in SOLIDWORKS MBD.

//--------------------------------------------------------------------------
// Preconditions: Open a part.
//
// Postconditions: None.
//--------------------------------------------------------------------------
using
SolidWorks.Interop.sldworks;
using
SolidWorks.Interop.swconst;
using
System.Runtime.InteropServices;
using
System;
namespace
GetGeneralTableAnno\_CSharp.csproj
{
    partial
class
SolidWorksMacro
    {

        ModelDoc2
Part;
        ModelDocExtension
modelDocExt;

        TableAnnotation
myTable;

        public
void Main()
        {
            Part = (ModelDoc2)swApp.**ActiveDoc**;
            modelDocExt = Part.**Extension**;
            myTable = modelDocExt.**GetGeneralTableAnnotation**(true,
0, 0, (int)swBOMConfigurationAnchorType\_e.swBOMConfigurationAnchor\_TopLeft,
"", 2,
2);

        }

        public
SldWorks
swApp;

    }
}