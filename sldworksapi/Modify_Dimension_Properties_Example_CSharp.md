<!-- source: sldworksapi/Modify_Dimension_Properties_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Modify Dimension Properties Example (C#)

This example shows how to modify the properties of a selected display
dimension in a drawing.

//------------------------------------------------------------
// Preconditions:
// 1. Open a drawing document with one or more display
//    dimensions.
// 2. Select a display dimension.
//
// Postconditions:
// 1. The properties of the selected display dimension
//
are modified
as specified.
// 2. Examine the display dimension to verify.
// -----------------------------------------------------------
using
SolidWorks.Interop.sldworks;
using
SolidWorks.Interop.swconst;
using
System.Runtime.InteropServices;
using
System;

namespace
ModifyDimensionProperties\_CSharp.csproj
{
    partial
class
SolidWorksMacro
    {

        ModelDoc2
swModel;

ModelDocExtension
swModelDocExt;

        bool
boolstatus;

        public
void Main()
        {
            swModel = (ModelDoc2)swApp.**ActiveDoc**;
            swModelDocExt
= (ModelDocExtension)swModel.Extension;

            boolstatus =
swModelDocExt.**EditDimensionProperties**((int)swTolType\_e.swTolBASIC,
0, 0, "",
"",
true, 9, (int)swDimensionArrowsSide\_e.swDimArrowsSmart,
false, (int)swArrowStyle\_e.swSLASH\_ARROWHEAD,
(int)swArrowStyle\_e.swSLASH\_ARROWHEAD,
"",
"",
true,
"",
"",
"Example of lower text",
true, (int)swInConfigurationOpts\_e.swThisConfiguration,
"");

            swModel.**ClearSelection2**(true);

        }

        public
SldWorks
swApp;

    }
}