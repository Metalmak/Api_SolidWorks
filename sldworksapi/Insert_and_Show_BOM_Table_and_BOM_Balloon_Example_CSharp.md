<!-- source: sldworksapi/Insert_and_Show_BOM_Table_and_BOM_Balloon_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Insert and Show BOM Table and BOM Balloon Example (C#)

This example shows how to insert a Bill of Materials (BOM) table and balloon in a
drawing document.

//----------------------------------------------------------------------------
// Preconditions:
// 1. Specified file and template exist.
// 2. Open an Immediate Window.
//
// Postconditions:
// 1. Inserts an indented BOM
table.
// 2. Inserts a BOM balloon annotation.
// 3. Inspect the Immediate
Window for the BOM feature properties.
//
// **NOTE**: Because the drawing is
used elsewhere, do not save any changes.
//---------------------------------------------------------------------------

using SolidWorks.Interop.sldworks;
using SolidWorks.Interop.swconst;
using System.Runtime.InteropServices;
using System;
using System.Diagnostics;

namespace IViewInsertBomTable4CSharp.csproj
{

    partial class SolidWorksMacro
    {

        public void Main()
        {
            ModelDoc2 swModel = default(ModelDoc2);
            ModelDocExtension swModelDocExt = default(ModelDocExtension);
            DrawingDoc swDrawing = default(DrawingDoc);
            View swView = default(View);
            BomTableAnnotation swBOMAnnotation = default(BomTableAnnotation);
            BomFeature swBOMFeature = default(BomFeature);
            Note swNote = default(Note);
            BalloonOptions BomBalloonParams = default(BalloonOptions);
            bool boolstatus = false;
            int AnchorType = 0;
            int NbrType = 0;
            int BomType = 0;
            int nErrors = 0;
            int nWarnings = 0;
            string Configuration = null;
            string TableTemplate = null;

            swModel = (ModelDoc2)swApp.**OpenDoc6**("C:\\Users\\Public\\Documents\\SOLIDWORKS\\SOLIDWORKS 2018\\samples\\tutorial\\advdrawings\\foodprocessor.slddrw", (int)swDocumentTypes\_e.swDocDRAWING, (int)swOpenDocOptions\_e.swOpenDocOptions\_Silent, "", ref nErrors, ref nWarnings);
            swDrawing = (DrawingDoc)swModel;
            swModelDocExt = (ModelDocExtension)swModel.**Extension**;
            boolstatus = swDrawing.**ActivateView**("Drawing View1");
            swView = (View)swDrawing.**ActiveDrawingView**;

            // Insert indented BOM table
            AnchorType = (int)swBOMConfigurationAnchorType\_e.swBOMConfigurationAnchor\_TopLeft;
            BomType = (int)swBomType\_e.swBomType\_Indented;
            NbrType = (int)swNumberingType\_e.swNumberingType\_Detailed;
            TableTemplate = "C:\\Program Files\\SOLIDWORKS Corp\\SOLIDWORKS\\lang\\english\\bom-standard.sldbomtbt";
            Configuration = "";
            swBOMAnnotation = (BomTableAnnotation)swView.**InsertBomTable4**(false, 0.4, 0.3, AnchorType, BomType, Configuration, TableTemplate, false, NbrType, true);
            swBOMFeature = (BomFeature)swBOMAnnotation.**BomFeature**;

            Debug.Print("Type of BOM table as defined in swBomType\_e: " + (int)swBOMFeature.**TableType**);

Debug.Print("Numbering type of BOM table as defined in swNumberingType\_e: " + (int)swBOMFeature.**NumberingTypeOnIndentedBOM**);

Debug.Print("Value to display when a value is 0 as defined in swZeroQuantityDisplay\_e: " + (int)swBOMFeature.**ZeroQuantityDisplay);**
            Debug.Print("Name of configuration used for BOM table: " + swBOMFeature.**Configuration**);
    Debug.Print("Display as one item? " + swBOMFeature.**DisplayAsOneItem**);

Debug.Print("Sequence start number: " + swBOMFeature.**SequenceStartNumber**);

Debug.Print("Keep missing items? " + swBOMFeature.**KeepMissingItems**);

Debug.Print("  Strikeout missing items? " + swBOMFeature.**StrikeoutMissingItems**);

Debug.Print("  Replace missing
components as defined in swKeepReplacedCompOption\_e: " + swBOMFeature.**KeepReplacedCompOption**);

Debug.Print("Keep current item numbers
when reordering rows? " + swBOMFeature.**KeepCurrentItemNumbers**);

            boolstatus = swModelDocExt.**SelectByID2**("", "EDGE", 0.1205506330468, 0.261655309417, -0.0004000000000133, false, 0, null, 0);

            BomBalloonParams = swModelDocExt.**CreateBalloonOptions**();
            BomBalloonParams.**Style** = (int)swBalloonStyle\_e.swBS\_Circular;
            BomBalloonParams.**Size** = (int)swBalloonFit\_e.swBF\_2Chars;
            BomBalloonParams.**UpperTextContent** = (int)swBalloonTextContent\_e.swBalloonTextItemNumber;
            BomBalloonParams.**ShowQuantity** = true;
            BomBalloonParams.**QuantityPlacement** = (int)swBalloonQuantityPlacement\_e.swBalloonQuantityPlacement\_Right;
            BomBalloonParams.**QuantityDenotationText** = "PLACES";
            BomBalloonParams.**QuantityOverride** = false;
            BomBalloonParams.**QuantityOverrideValue** = "";
            BomBalloonParams.**ItemNumberStart** = 1;
            BomBalloonParams.**ItemNumberIncrement** = 1;
            BomBalloonParams.**ItemOrder** = (int)swBalloonItemNumbersOrder\_e.swBalloonItemNumbers\_DoNotChangeItemNumbers;

            swNote = (Note)swModelDocExt.**InsertBOMBalloon2**(BomBalloonParams);

            if (swNote.**IsBomBalloon**())
            {
                Debug.Print("Name of BOM balloon: " + swNote.**GetName**());
            }

            swDrawing.Force**R**ebuild();

        }

        public SldWorks swApp;

    }
}