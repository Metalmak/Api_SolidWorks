<!-- source: sldworksapi/Insert_General_Table_in_Part_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Insert General Table in Part Example (C#)

This example shows how to insert a general table annotation into a model
document.

//---------------------------------------------------
// Preconditions: Open a part.
//
// Postconditions:
// 1. Inserts a general table in the part.
// 2. Examine the graphics area.
//---------------------------------------------------
using
SolidWorks.Interop.sldworks;
using
SolidWorks.Interop.swconst;
using
System.Runtime.InteropServices;
using
System;
namespace
InsertGeneralTable\_CSharp.csproj
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
            myTable = modelDocExt.**InsertGeneralTableAnnotation**(true,
0, 0, (int)swBOMConfigurationAnchorType\_e.swBOMConfigurationAnchor\_TopLeft,
"", 2,
2);

        }

        public
SldWorks
swApp;

    }
}