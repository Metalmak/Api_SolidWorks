<!-- source: swutilitiesapi/Compare_Geometry_CSharp.htm -->

# SOLIDWORKS Utilities API Help

# Compare Geometry Example (C#)

This example shows how to use the SOLIDWORKS Utilities API to compare
geometries in two part documents.

```
'---------------------------------------------------------------------------------
' Preconditions:
' 1. Add the SOLIDWORKS Utilities as an add-in
'    (in SOLIDWORKS, click Tools > Add-Ins > SOLIDWORKS Utilities).
' 2. Add the SOLIDWORKS Utilities interop assembly as a reference
'    (right-click the project in Project Explorer, click Add Reference >
'     browse to install_dir\api\redist > Solidworks.Interop.gtswutilities.dll).
' 3. Verify that the specified files exist.
' 4. Verify that C:\test\ exists.
' 5. Open the Immediate window.
'
' Postconditions:
' 1. Creates C:\test\Report\gtReportIndex.htm.
' 2. Gets the face and volume comparison statuses.
' 3. Examine the Immediate window, graphics area, and
'    C:\test\report\gtReportIndex.htm.
'
' NOTE: Because the parts are used elsewhere, do not save changes.
'--------------------------------------------------------------------------------
```

using SOLIDWORKS.Interop.sldworks;

using SOLIDWORKS.Interop.swconst;

using SOLIDWORKS.Interop.gtswutilities;

using System;

using System.Diagnostics;

namespace CompareGeometry\_CSharp.csproj

{

    partial
class SOLIDWORKSMacro

    {

        public
void Main()

        {

            gtcocswUtilities
swUtil = default(gtcocswUtilities);

            gtcocswCompareGeometry
swUtilCompGeom = default(gtcocswCompareGeometry);

            gtError\_e
longStatus = default(gtError\_e);

            bool
bAddToBinder = false;

            bool
bOverwrite = false;

            int
errorCode = 0;

            //
Get the SOLIDWORKS Utilities tool interface

            swUtil
= (gtcocswUtilities)swApp.**GetAddInObject**("Utilities.UtilitiesApp");

            //
Get the CompareGeometry tool

            swUtilCompGeom
= (gtcocswCompareGeometry)swUtil.GetToolInterface(2,
out errorCode);

            if
(!(errorCode == (int)gtError\_e.gtNOErr))

            {

                Debug.Print("Error
getting compare geometry tool.");

            }

            //
Compare the volumes and faces of the specified part documents

            //
Save the results to a file in the specified path

            bAddToBinder
= false;

            bOverwrite
= true;

            string
file1 = null;

            string
file2 = null;

            int
volDiffStatus = 0;

            int
faceDiffStatus = 0;

            file1
= "C:\\Users\\Public\\Documents\\SOLIDWORKS\\SOLIDWORKS 2018\\samples\\tutorial\\swutilities\\bracket\_a.sldprt";

            file2
= "C:\\Users\\Public\\Documents\\SOLIDWORKS\\SOLIDWORKS 2018\\samples\\tutorial\\swutilities\\bracket\_b.sldprt";

            longStatus
= (gtError\_e)swUtilCompGeom.CompareGeometry3(file1,
"", file2, "", (int)gtGdfOperationOption\_e.gtGdfFaceAndVolumeCompare,
(int)gtResultOptions\_e.gtResultSaveReport, "C:\\test\\Report",
bAddToBinder, bOverwrite, ref volDiffStatus,

            ref
faceDiffStatus);

            if
(!(longStatus == gtError\_e.gtNOErr))

            {

                Debug.Print("Error
comparing geometries.");

            }

            diffStatus("Volume
comparison", volDiffStatus);

            diffStatus("Face
comparison", faceDiffStatus);

            //
Perform any necessary clean up

            longStatus
= (gtError\_e)swUtilCompGeom.Close();

        }

        public
void diffStatus(string name, int diffCode)

        {

            Debug.Print(name);

            switch
(diffCode)

            {

                case
(int)gtVolDiffStatusOptionType\_e.gtSuccess:

                    Debug.Print("Succeeded");

                    break;

                case
(int)gtVolDiffStatusOptionType\_e.gtNotPerformed:

                    Debug.Print("Not
performed");

                    break;

                case
(int)gtVolDiffStatusOptionType\_e.gtCanceled:

                    Debug.Print("Canceled");

                    break;

                case
(int)gtVolDiffStatusOptionType\_e.gtFailed:

                    Debug.Print("Failed");

                    break;

                case
(int)gtVolDiffStatusOptionType\_e.gtIdenticalParts:

                    Debug.Print("Identical
parts");

                    break;

                case
(int)gtVolDiffStatusOptionType\_e.gtDifferentParts:

                    Debug.Print("Different
parts");

                    break;

                case
(int)gtVolDiffStatusOptionType\_e.gtNoSolidBody:

                    Debug.Print("No
solid body found");

                    break;

                case
(int)gtVolDiffStatusOptionType\_e.gtAlreadySaved:

                    Debug.Print("Already
saved");

                    break;

            }

            Debug.Print("
");

        }

        public
SldWorks swApp;

    }

}