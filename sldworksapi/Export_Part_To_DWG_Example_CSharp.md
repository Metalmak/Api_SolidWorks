<!-- source: sldworksapi/Export_Part_To_DWG_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Export Part to DWG Example (C#)

This example shows how to export sheet metal and annotation views of a part
to DWG files.

//---------------------------------------------------------------------------
// Preconditions: Copy *public\_documents***\samples\tutorial\api\2012-sm.sldprt** to
// **c:\temp**.
//
// Postconditions:
// 1. Creates three DWG files containing:
//    \* Current annotation view
//    \* Front annotation view
//    \* flat-pattern sheet metal
// 2. Locate and open the just-created DWG files in **c:\temp**.
//--------------------------------------------------------------------------
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
ExportToDWG2\_CSharp.csproj
{
    partial
class
SolidWorksMacro
    {

        ModelDoc2
swModel;
        PartDoc
swPart;
        string
sModelName;
        string
sPathName;
        object
varAlignment;
        double[]
dataAlignment = new
double[12];
        object
varViews;
        string[]
dataViews = new
string[2];

        int
options;

        public
void Main()
        {
            swModel = (ModelDoc2)swApp.**ActiveDoc**;

            sModelName = swModel.**GetPathName**();
            sPathName = swModel.**GetPathName**();
            sPathName = sPathName.Substring(0, sPathName.Length - 6);
            sPathName = sPathName + "dwg";

            swPart = (PartDoc)swModel;

            dataAlignment[0] = 0.0;
            dataAlignment[1] = 0.0;
            dataAlignment[2] = 0.0;
            dataAlignment[3] = 1.0;
            dataAlignment[4] = 0.0;
            dataAlignment[5] = 0.0;
            dataAlignment[6] = 0.0;
            dataAlignment[7] = 1.0;
            dataAlignment[8] = 0.0;
            dataAlignment[9] = 0.0;
            dataAlignment[10] = 0.0;
            dataAlignment[11] = 1.0;

            varAlignment = dataAlignment;

            dataViews[0] = "\*Current";
            dataViews[1] = "\*Front";

            varViews = dataViews;

            //Export each annotation view
to a separate drawing file
            swPart.**ExportToDWG2**(sPathName,
sModelName, (int)swExportToDWG\_e.swExportToDWG\_ExportAnnotationViews, false,
varAlignment, false,
false, 0,
varViews);

            //Export sheet metal to a
single drawing file
            options = 1;
 //include flat-pattern geometry
            swPart.**ExportToDWG2**(sPathName,
sModelName, (int)swExportToDWG\_e.swExportToDWG\_ExportSheetMetal, true,
varAlignment, false,
false,
options, null);

        }

        public
SldWorks
swApp;

    }

}