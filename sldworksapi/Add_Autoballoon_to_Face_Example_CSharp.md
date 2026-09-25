<!-- source: sldworksapi/Add_Autoballoon_to_Face_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Add Auto Balloons to Drawing Example (C#)

This example shows how to automatically add BOM balloons to a drawing view.

//------------------------------------------------------------------------------
// Preconditions: Open a drawing with a bill of materials (BOM) table.
//
// Postconditions: BOM balloons are added to the view.
//------------------------------------------------------------------------------
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
AutoBalloon\_CSharp.csproj
{
    partial
class
SolidWorksMacro
    {
        ModelDoc2
Part;
        DrawingDoc
Draw;
        object
vNotes;
        AutoBalloonOptions
autoballoonParams;

        bool
boolstatus;

        public
void Main()
        {
            Part = (ModelDoc2)swApp.ActiveDoc;
            Draw = (DrawingDoc)Part;
            boolstatus = Draw.ActivateView("Drawing
View1");
            boolstatus = Part.Extension.SelectByID2("Drawing
View1",
"DRAWINGVIEW", 0, 0, 0,
false, 0,
null, 0);

            autoballoonParams = Draw.CreateAutoBalloonOptions();
            autoballoonParams.Layout = (int)swBalloonLayoutType\_e.swDetailingBalloonLayout\_Square;
            autoballoonParams.ReverseDirection =
false;
            autoballoonParams.IgnoreMultiple =
true;
            autoballoonParams.InsertMagneticLine =
true;
            autoballoonParams.LeaderAttachmentToFaces =
true;
            autoballoonParams.Style = (int)swBalloonStyle\_e.swBS\_Circular;
            autoballoonParams.Size = (int)swBalloonFit\_e.swBF\_5Chars;
            autoballoonParams.UpperTextContent = (int)swBalloonTextContent\_e.swBalloonTextItemNumber;
            autoballoonParams.Layername =
"-None-";
            autoballoonParams.ItemNumberStart = 1;
            autoballoonParams.ItemNumberIncrement = 1;
            autoballoonParams.ItemOrder = (int)swBalloonItemNumbersOrder\_e.swBalloonItemNumbers\_DoNotChangeItemNumbers;

autoballoonParams.EditBalloons =
true;

autoballoonParams.EditBalloonOption = (int)swEditBalloonOption\_e.swEditBalloonOption\_Resequence;

            vNotes = Draw.AutoBalloon5(autoballoonParams);

        }

        public
SldWorks
swApp;

    }
}