<!-- source: sldworksapi/Set_Rounding_of_Decimal_Units_in_Display_Dimensions_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Set Rounding of Decimal Units in Display Dimensions (C#)

This example shows how to specify the rounding of decimal units in display
dimensions.

//----------------------------------------------------------------------------
// Preconditions: Open:
//    *public\_documents***\samples\tutorial\api\box.slddrw**
//
// Postconditions:
// 1. Click the display dimension in the graphics area.
// 2. Under **Dual Dimension** on the Value tab, observe that **Inward
rounding**
//    is selected.
// 3. Under **Override Units** on the Other tab, observe that:
//    \* **Decimal** is clicked.
//    \* **Feet & Inches** is selected.
//    \* **Truncate without rounding** is selected.
//
// NOTE: Because the model is used elsewhere,
// do not save changes when closing it.
//
---------------------------------------------------------------------------
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
SetDual2\_CSharp.csproj
{
    partial
class
SolidWorksMacro
    {

        ModelDoc2
Part;
        SelectionMgr
swSelMgr;
        DisplayDimension
swDispDim;
        bool
boolstatus;

        int
longstatus;

        public
void Main()
        {
            Part = (ModelDoc2)swApp.**ActiveDoc**;

            swSelMgr = (SelectionMgr)Part.**SelectionManager**;
            boolstatus = Part.**Extension**.**SelectByID2**("RD1@Drawing
View1",
"DIMENSION", 0.305961854224123,
0.247549077953509, 0, false,
0, null,
0);
            swDispDim = (DisplayDimension)swSelMgr.**GetSelectedObject6**(1,
0);

            longstatus = swDispDim.**SetUnits2**(false,
(int)swLengthUnit\_e.swFEETINCHES,
(int)swFractionDisplay\_e.swDECIMAL,
0, false, (int)swUnitsDecimalRounding\_e.swUnitsDecimalRounding\_Truncate);
            swDispDim.**SetDual2**(false,
true);

        }

        public
SldWorks
swApp;

    }

}