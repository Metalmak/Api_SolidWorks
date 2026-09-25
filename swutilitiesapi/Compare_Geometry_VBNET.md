<!-- source: swutilitiesapi/Compare_Geometry_VBNET.htm -->

# SOLIDWORKS Utilities API Help

# Compare Geometry Example (VB.NET)

This example shows how to use the SOLIDWORKS Utilities API to compare
geometries in two part documents.

```
'---------------------------------------------------------------------------------
' Preconditions:
' 1. Add the SOLIDWORKS Utilities as an add-in
'    (in SOLIDWORKS, click Tools > Add-Ins > SOLIDWORKS Utilities).
' 2. Add the SOLIDWORKS Utilities interop assembly as a reference
'    (right-click the project in Project Explorer, click Add Reference >
'     browse to install_dir\api\redist > SolidWorks.Interop.gtswutilities.dll).
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

Imports SOLIDWORKS.Interop.sldworks

Imports SOLIDWORKS.Interop.swconst

Imports SOLIDWORKS.Interop.gtswutilities

Imports System

Imports System.Diagnostics

Partial Class SOLIDWORKSMacro

    Sub
main()

        Dim
swUtil As gtcocswUtilities

        Dim
swUtilCompGeom As gtcocswCompareGeometry

        Dim
longStatus As gtError\_e

        Dim
bAddToBinder As Boolean

        Dim
bOverwrite As Boolean

        Dim
errorCode As Integer

        '
Get the SOLIDWORKS Utilities tool interface

        swUtil
= swapp.**GetAddInObject**("Utilities.UtilitiesApp")

        '
Get the CompareGeometry tool

        swUtilCompGeom
= swUtil.GetToolInterface(2, errorCode)

        If
Not errorCode = gtError\_e.gtNOErr Then

            Debug.Print("Error
getting compare geometry tool.")

        End
If

        '
Compare the volumes and faces of the specified part documents

        bAddToBinder
= False

        bOverwrite
= True

        Dim
file1 As String

        Dim
file2 As String

        Dim
volDiffStatus As Integer

        Dim
faceDiffStatus As Integer

        file1
= "C:\Users\Public\Documents\SOLIDWORKS\SOLIDWORKS 2018\samples\tutorial\swutilities\bracket\_a.sldprt"

        file2
= "C:\Users\Public\Documents\SOLIDWORKS\SOLIDWORKS 2018\samples\tutorial\swutilities\bracket\_b.sldprt"

        longStatus
= swUtilCompGeom.CompareGeometry3(file1,
"", file2, "", gtGdfOperationOption\_e.gtGdfFaceAndVolumeCompare,
gtResultOptions\_e.gtResultSaveReport, "C:\test\Report", bAddToBinder,
bOverwrite, volDiffStatus, faceDiffStatus)

        If
Not longStatus = gtError\_e.gtNOErr Then

            Debug.Print("Error
comparing geometries.")

        End
If

        Call
diffStatus("Volume comparison", volDiffStatus)

        Call
diffStatus("Face comparison", faceDiffStatus)

        '
Perform any necessary clean up

        longStatus
= swUtilCompGeom.Close()

    End
Sub

    Sub
diffStatus(ByVal name As String, ByVal diffCode As gtVolDiffStatusOptionType\_e)

        Debug.Print(name)

        Select
Case diffCode

            Case
gtVolDiffStatusOptionType\_e.gtSuccess

                Debug.Print("Succeeded")

            Case
gtVolDiffStatusOptionType\_e.gtNotPerformed

                Debug.Print("Not
performed")

            Case
gtVolDiffStatusOptionType\_e.gtCanceled

                Debug.Print("Canceled")

            Case
gtVolDiffStatusOptionType\_e.gtFailed

                Debug.Print("Failed")

            Case
gtVolDiffStatusOptionType\_e.gtIdenticalParts

                Debug.Print("Identical
parts")

            Case
gtVolDiffStatusOptionType\_e.gtDifferentParts

                Debug.Print("Different
parts")

            Case
gtVolDiffStatusOptionType\_e.gtNoSolidBody

                Debug.Print("No
solid body found")

            Case
gtVolDiffStatusOptionType\_e.gtAlreadySaved

                Debug.Print("Already
saved")

        End
Select

    End
Sub

    Public
swApp As SldWorks

End Class