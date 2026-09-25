<!-- source: sldworksapi/Create_Layer_for_Selected_View_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Create Layer for Selected View Example (C#)

This example shows how to create a layer for the part in the selected drawing view.

//----------------------------------------------------------------------------
// Preconditions:
// 1. Open a drawing of a part.
// 2. Add a reference to **Microsoft.VisualBasic**.
// 3. Select a drawing view in the FeatureManager design tree.
// 4. Open the Immediate window.
//
// Postconditions:
// 1. Creates a layer for the part in the selected drawing view.
// 2. Click the **Layer Properties** tool on the Line Format toolbar to verify
//    that the newly created layer is selected in the Layers dialog box.
// 3. Examine the Immediate window.
//----------------------------------------------------------------------------
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
CreateLayer2\_CSharp.csproj
{
    partial
class
SolidWorksMacro
    {

        private
void
ChangeComponentLayer(DrawingDoc
swDraw, string
sLayerName)
        {
            bool
bRet = false;

            // Form a valid layer name
            sLayerName =
Strings.Replace(sLayerName,
"/",
"\_", 1,
-1, 0);
            sLayerName = Strings.Replace(sLayerName,
"@",
"\_", 1,
-1, 0);

            bRet = swDraw.**CreateLayer2**(sLayerName,
"Layer for part in "
+ sLayerName, 0, (int)swLineStyles\_e.swLineCONTINUOUS,
(int)swLineWeights\_e.swLW\_NORMAL,
true,
true);

            // Change in all views
            swDraw.**ChangeComponentLayer**(sLayerName,
true);

        }

        public
void Main()
        {
            ModelDoc2
swModel = default(ModelDoc2);
            DrawingDoc
swDraw = default(DrawingDoc);
            SelectionMgr
swSelMgr = default(SelectionMgr);
            View
swView = default(View);
            ModelDoc2
swDrawModel = default(ModelDoc2);
            PartDoc
swDrawPart = default(PartDoc);
            int
nErrors = 0;
            int
nWarnings = 0;

            swModel = (ModelDoc2)swApp.**ActiveDoc**;
            swDraw = (DrawingDoc)swModel;
            swSelMgr = (SelectionMgr)swModel.**SelectionManager**;
            swView = (View)swSelMgr.**GetSelectedObject6**(1,
-1);
            swDrawModel = swApp.**OpenDoc6**(swView.**GetReferencedModelName**(),
(int)swDocumentTypes\_e.swDocPART,
(int)swOpenDocOptions\_e.swOpenDocOptions\_Silent,
"",
ref nErrors,
ref
nWarnings);
            swDrawPart = (PartDoc)swDrawModel;

            Debug.Print("File
= " + swModel.**GetPathName**());
            Debug.Print("  View
= " + swView.**Name**);
            Debug.Print("    View
Model = " + swView.**GetReferencedModelName**());

            ChangeComponentLayer(swDraw, swView.**Name**);

        }

        public
SldWorks
swApp;

    }

}