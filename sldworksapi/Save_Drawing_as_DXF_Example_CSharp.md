<!-- source: sldworksapi/Save_Drawing_as_DXF_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Save Drawing as DXF Example (C#)

This example shows how to save the current drawing file as a DXF file
in the same folder.

//----------------------------------------------------------------------------
// Preconditions:
// 1. Open a drawing.
// 2. Open the Immediate window.
//
// Postconditions:
// 1. Gets and sets DXF-related system settings.
// 2. Saves the drawing as a DXF file in the same folder as the drawing,
//    overwriting any existing file of the same name.
// 3. Examine the Immediate window and the folder to which the DXF file
//    was saved.
//----------------------------------------------------------------------------

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
SaveDrawingAsDXF\_CSharp.csproj
{
    partial
class
SolidWorksMacro
    {

        ModelDoc2
swModel;
        string
sPathName;
        int
nErrors;
        int
nWarnings;
        int
nRetval;
        bool
bShowMap;

        bool
bRet;

        public
void Main()
        {
            swModel = (ModelDoc2)swApp.**ActiveDoc**;

            // Strip off SOLIDWORKS drawing
file extension (.slddrw)
            //
and add DXF file extension (.dxf)
            sPathName = swModel.**GetPathName**();
            sPathName = sPathName.Substring(0, sPathName.Length - 6);
            sPathName = sPathName + "dxf";
            Debug.Print(sPathName);

            // Show current settings
            Debug.Print("DxfMapping
= " + swApp.**GetUserPreferenceToggle**((int)swUserPreferenceToggle\_e.swDxfMapping));
            Debug.Print("DXFDontShowMap
= " + swApp.**GetUserPreferenceToggle**((int)swUserPreferenceToggle\_e.swDXFDontShowMap));
            Debug.Print("DxfVersion
= " + swApp.**GetUserPreferenceIntegerValue**((int)swUserPreferenceIntegerValue\_e.swDxfVersion));
            Debug.Print("DxfOutputFonts
= " + swApp.**GetUserPreferenceIntegerValue**((int)swUserPreferenceIntegerValue\_e.swDxfOutputFonts));
            Debug.Print("DxfMappingFileIndex    =
" + swApp.**GetUserPreferenceIntegerValue**((int)swUserPreferenceIntegerValue\_e.swDxfMappingFileIndex));
            Debug.Print("DxfOutputLineStyles    =
" + swApp.**GetUserPreferenceIntegerValue**((int)swUserPreferenceIntegerValue\_e.swDxfOutputLineStyles));
            Debug.Print("DxfOutputNoScale
= " + swApp.**GetUserPreferenceIntegerValue**((int)swUserPreferenceIntegerValue\_e.swDxfOutputNoScale));
            Debug.Print("DxfMappingFiles        =
" + swApp.**GetUserPreferenceStringListValue**((int)swUserPreferenceStringListValue\_e.swDxfMappingFiles));
            Debug.Print("DxfOutputScaleFactor
= " + swApp.**GetUserPreferenceDoubleValue**((int)swUserPreferenceDoubleValue\_e.swDxfOutputScaleFactor));
            Debug.Print("");

            // Turn off showing of map
            bShowMap = swApp.**GetUserPreferenceToggle**((int)swUserPreferenceToggle\_e.swDXFDontShowMap);
            Debug.Print("bShowMap
= " + bShowMap);

            swApp.**SetUserPreferenceToggle**((int)swUserPreferenceToggle\_e.swDXFDontShowMap,
false);

            bRet = swModel.**SaveAs4**(sPathName, (int)swSaveAsVersion\_e.swSaveAsCurrentVersion,
(int)swSaveAsOptions\_e.swSaveAsOptions\_Silent,
ref nErrors,
ref
nWarnings);

            if
(bRet == false)
            {
                nRetval = swApp.**SendMsgToUser2**("Problems
saving file.", (int)swMessageBoxIcon\_e.swMbWarning,
(int)swMessageBoxBtn\_e.swMbOk);
            }

            // Restore showing of map
            swApp.**SetUserPreferenceToggle**((int)swUserPreferenceToggle\_e.swDXFDontShowMap,
bShowMap);

        }

        public
SldWorks
swApp;

    }

}