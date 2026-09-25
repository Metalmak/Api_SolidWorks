<!-- source: sldworksapi/Select_All_in_Part_Assembly_or_Drawing_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Select All in Part, Assembly, or Drawing (C#)

This example shows how to select everything in the graphics area of a part or
assembly document or in the sheet of a drawing document, as if you box-selected everything in the graphics area or
the sheet.

//--------------------------------------------------------------------------
// Preconditions:
// 1. Verify that the part, assembly, and drawing documents opened by the macro
//    exist.
// 2. Open the Immediate window.
//
// Postconditions:
// 1. Examine:
//    \* Sheet to verify that all of the entities in the drawing
//      are selected.
//    \* Immediate window to see how many entities are selected.
// 2. Click **Window > bolt-assembly.sldasm** to switch to the assembly
//    document.
// 3. Examine:
//    \* Graphics area to verify that the all of the components
//      in the assembly are selected.
//    \* Immediate window to see how many components are selected.
// 4. Click **Window > bolt.sldprt** to switch to the part document.
// 5. Examine:
//    \* Graphics area to verify that the all of the edges
//      in the part are selected.
//    \* Immediate window to see how many edges are selected.
//
// NOTE: Because these documents are used elsewhere, do not save changes.
//--------------------------------------------------------------------------

using
SolidWorks.Interop.sldworks;
using
SolidWorks.Interop.swconst;
using
System;
using
System.Diagnostics;

namespace
SelectAllModelDocExtensionCSharp.csproj
{
    partial
class
SolidWorksMacro
    {

        public
void
Main()
        {
            ModelDoc2 swModel;
            ModelDocExtension swModelDocExt;
            SelectionMgr swSelMgr;
            string
partFile = null;
            string
assemblyFile = null;
            string
drawingFile = null;
            int
errors = 0;
            int
warnings = 0;

            // Open a part document and
select all edges in the part
            partFile =
"C:\\Users\\Public\\Documents\\SOLIDWORKS\\SOLIDWORKS 2017\\introsw\\bolt.sldprt";
            swModel = (ModelDoc2)swApp.**OpenDoc6**(partFile, (int)swDocumentTypes\_e.swDocPART,
(int)swOpenDocOptions\_e.swOpenDocOptions\_Silent,
"",
ref
errors, ref
warnings);
            swModelDocExt = (ModelDocExtension)swModel.**Extension**;
            swSelMgr = (SelectionMgr)swModel.**SelectionManager**;
            //Select all edges in part
            SelectAllinDocument(swModel,
swModelDocExt, swSelMgr);

            // Open an assembly
document and select all components in the assembly
            assemblyFile =
"C:\\Users\\Public\\Documents\\SOLIDWORKS\\SOLIDWORKS 2017\\introsw\\bolt-assembly.sldasm";
            swModel = (ModelDoc2)swApp.**OpenDoc6**(assemblyFile, (int)swDocumentTypes\_e.swDocASSEMBLY,
(int)swOpenDocOptions\_e.swOpenDocOptions\_Silent,
"",
ref
errors, ref
warnings);
            swModelDocExt = (ModelDocExtension)swModel.**Extension**;
            swSelMgr = (SelectionMgr)swModel.**SelectionManager**;
            //Select all components in
assembly
            SelectAllinDocument(swModel,
swModelDocExt, swSelMgr);

            // Open a drawing document
and select all entities in the drawing
            drawingFile =
"C:\\Users\\Public\\Documents\\SOLIDWORKS\\SOLIDWORKS 2017\\introsw\\bolt-assembly.slddrw";
            swModel = (ModelDoc2)swApp.**OpenDoc6**(drawingFile, (int)swDocumentTypes\_e.swDocDRAWING,
(int)swOpenDocOptions\_e.swOpenDocOptions\_Silent,
"",
ref
errors, ref
warnings);
            swModelDocExt = (ModelDocExtension)swModel.**Extension**;
            swSelMgr = (SelectionMgr)swModel.**SelectionManager**;
            //Select all entities in
drawing
            SelectAllinDocument(swModel,
swModelDocExt, swSelMgr);

        }

        public
void
SelectAllinDocument(ModelDoc2 swModel, ModelDocExtension swModelDocExt,
SelectionMgr swSelMgr)
        {
            int
selCount;

            // Select all edges in a
part, all components in an assembly,
            //
or all entities in a drawing
            swModelDocExt.**SelectAll**();

            // Get and print the number
of selections
            selCount = 0;
            selCount = swSelMgr.**GetSelectedObjectCount2**(-1);

            switch
(swModel.**GetType**())
            {
                case
(int)swDocumentTypes\_e.swDocPART:
                    Debug.Print("Number
of edges selected in part          = "
+ selCount);
                    break;
                case
(int)swDocumentTypes\_e.swDocASSEMBLY:
                    Debug.Print("Number
of components selected in assembly = "
+ selCount);
                    break;
                case
(int)swDocumentTypes\_e.swDocDRAWING:
                    Debug.Print("Number
of entities selected in drawing    = "
+ selCount);
                    break;
                default:
                    Debug.Print("Unknown
type of document.");
                    break;
            }

        }

        ///
<summary>
        ///
The SldWorks swApp variable is pre-assigned for you.
        ///
</summary>
        public
SldWorks swApp;

    }
}