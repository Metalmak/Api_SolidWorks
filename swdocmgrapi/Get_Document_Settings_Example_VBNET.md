<!-- source: swdocmgrapi/Get_Document_Settings_Example_VBNET.htm -->

# SOLIDWORKS Document Manager API Help

# Get Document Settings Example (VB.NET)

This example shows how to get various settings for a document.

'---------------------------------------------------------------------------------------
' Preconditions:
' 1. Read the SOLIDWORKS Document Manager API **Getting Started**

'    topic and ensure that the required DLLs are registered.
' 2. Copy and paste this code into a VB.NET console application
'    in Microsoft Visual Studio.
' 3. Add the **SolidWorks.Interop.swdocumentmgr.dll** reference to the project:

'    a. Right-click the solution in Solution Explorer.
'    b. Select **Add Reference**.
'    c. Click **Browse**.
'    d. Click *install\_dir***\api\redist\SolidWorks.Interop.swdocumentmgr.dll**.
'    e. Click **Add**.
'    f. Click **Close**.
' 4. Substitute *path\_to\_SOLIDWORKS\_2015\_model* with the path to a
model that has been
'    saved in SOLIDWORKS 2015 or later.
' 5. Substitute *your\_license\_key* with your SOLIDWORKS Document Manager
'    license key.
' 6. Open the Immediate window.
'
' Postconditions: Examine the Immediate window.
'

' NOTE: Because the model is used elsewhere, do not save any changes.

'---------------------------------------------------------------------------------------

Imports SolidWorks.Interop.swdocumentmgr
Imports System
Imports System.Diagnostics

Module Module1

    Dim dmClassFact As SwDMClassFactory
    Dim dmDocMgr As SwDMApplication4
    Dim dmDoc As SwDMDocument19
    Dim dmDocType As SwDmDocumentType
    Dim status As SwDmDocumentOpenError

    Const docPath As String = "*path\_to\_SOLIDWORKS\_2015\_model*"
    Const licenseKey As String = "*your\_license\_key*"

    Sub main()

        dmClassFact = CreateObject("SwDocumentMgr.SwDMClassFactory")
        dmDocMgr = dmClassFact.**GetApplication**(licenseKey)
        dmDoc = dmDocMgr.**GetDocument**(docPath, dmDocType, True, status)

        If Not (dmDoc Is Nothing) Then
            Debug.Print("Angular units: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsAngular))
            Debug.Print("Angular decimal places: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsAngularDecimalPlaces))
            Debug.Print("Decimal rounding: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsDecimalRounding))
            Debug.Print("Dual linear units: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsDualLinear))
            Debug.Print("Dual linear decimal display: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsLinearDecimalDisplay))
            Debug.Print("Dual linear decimal places: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsLinearDecimalPlaces))
            Debug.Print("Dual linear fraction denominator: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsDualLinearFractionDenominator))
            Debug.Print("Energy decimal places: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsEnergyDecimalPlaces))
            Debug.Print("Energy units: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsEnergyUnits))
            Debug.Print("Force units: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsForce))
            Debug.Print("Force decimal places: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsForceDecimalPlaces))
            Debug.Print("Linear units: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsLinear))
            Debug.Print("Linear decimal display: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsLinearDecimalDisplay))
            Debug.Print("Linear decimal places: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsLinearDecimalPlaces))
            Debug.Print("Linear fraction denominator: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsLinearFractionDenominator))
            Debug.Print("Mass prop decimal places: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsMassPropDecimalPlaces))
            Debug.Print("Mass prop length: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsMassPropLength))
            Debug.Print("Mass prop mass: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsMassPropMass))
            Debug.Print("Mass prop volume: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsMassPropVolume))
            Debug.Print("Power decimal places: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsPowerDecimalPlaces))
            Debug.Print("Power units: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsPowerUnits))
            Debug.Print("Time decimal places: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsTimeDecimalPlaces))
            Debug.Print("Time units: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsTimeUnits))
            Debug.Print("Unit system: " & dmDoc.**GetSwDmSettingInteger**(swDmDocumentUnitsIntegerValue\_e.swDmUnitsUnitSystem))

            Debug.Print("Dual linear feet and inches format? " & dmDoc.**GetSwDmSettingToggle**(swDmDocumentUnitsToggle\_e.swDmUnitsDualLinearFeetAndInchesFormat))
            Debug.Print("Dual linear round to nearest fraction? " & dmDoc.**GetSwDmSettingToggle**(swDmDocumentUnitsToggle\_e.swDmUnitsDualLinearRoundToNearestFraction))
            Debug.Print("Linear feet and inches format? " & dmDoc.**GetSwDmSettingToggle**(swDmDocumentUnitsToggle\_e.swDmUnitsLinearFeetAndInchesFormat))
            Debug.Print("Linear round to nearest fraction? " & dmDoc.**GetSwDmSettingToggle**(swDmDocumentUnitsToggle\_e.swDmUnitsLinearRoundToNearestFraction))

        Else
            Debug.Print("Unable to open document. Check docPath variable.")
        End If

    End Sub

End Module