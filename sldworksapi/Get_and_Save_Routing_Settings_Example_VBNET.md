<!-- source: sldworksapi/Get_and_Save_Routing_Settings_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Get and Save Routing Settings Example (VB.NET)

This example shows how to get and save routing settings.

'----------------------------------------------------------------------------
' Preconditions:
' 1. In SOLIDWORKS, click **Tools > Add-Ins**,
select **SOLIDWORKS Routing**, and'    click **OK**.
'
2. In
the IDE, right-click the project, select **Add Reference**,
'

browse *install\_dir***\api\redist**, and click

'    **SolidWorks.Interop.SWRoutingLib.dll**.

' 3. Ensure that **c:\temp** exists.
' 4. Open an Immediate window.
'
' Postconditions:
' 1. Saves routing settings to **c:\temp\routingSettings.sqy**.
' 2. Inspect the Immediate window.

'---------------------------------------------------------------------------
Imports SolidWorks.Interop.sldworks
Imports SolidWorks.Interop.swconst
Imports SolidWorks.Interop.SWRoutingLib
Imports System.Runtime.InteropServices
Imports System
Imports System.Diagnostics

Partial Class SolidWorksMacro

    Sub main()

        Dim routingSettings As RoutingSettings
        Dim boolstatus As Integer

        Dim wireNameHdr As String, fromRefHdr As String, fromPinHdr As String, fromPartNoHdr As String, toRefHdr As String, toPinHdr As String, toPartNoHdr As String, cableNameHdr As String, coreNameHdr As String, colourHdr As String, wireSpecHdr As String, otherAttribHdr As String
        wireNameHdr = ""
        fromRefHdr = ""
        fromPinHdr = ""
        fromPartNoHdr = ""
        toRefHdr = ""
        toPinHdr = ""
        toPartNoHdr = ""
        cableNameHdr = ""
        coreNameHdr = ""
        colourHdr = ""
        wireSpecHdr = ""
        otherAttribHdr = ""

        routingSettings = swApp.**GetRoutingSettings**

        boolstatus = routingSettings.**SaveRoutingSettingsToFile**("c:\temp\routingSettings.sqy")
        boolstatus = routingSettings.**GetFromToListHeaderDefinitions**(wireNameHdr, fromRefHdr, fromPinHdr, fromPartNoHdr, toRefHdr, toPinHdr, toPartNoHdr, cableNameHdr, coreNameHdr, colourHdr, wireSpecHdr, otherAttribHdr)
        Debug.Print("From-to list column headers")
        Debug.Print("  Wire name: " & wireNameHdr)
        Debug.Print("  From reference: " & fromRefHdr)
        Debug.Print("  From pin: " & fromPinHdr)
        Debug.Print("  From part number: " & fromPartNoHdr)
        Debug.Print("  To reference: " & toRefHdr)
        Debug.Print("  To pin: " & toPinHdr)
        Debug.Print("  To part number: " & toPartNoHdr)
        Debug.Print("  Cable name: " & cableNameHdr)
        Debug.Print("  Core name: " & coreNameHdr)
        Debug.Print("  Color: " & colourHdr)
        Debug.Print("  Wire spec: " & wireSpecHdr)
        Debug.Print("  Other attribute: " & otherAttribHdr)
        Debug.Print("")
        Debug.Print("Slack %: " & routingSettings.**GetRoutingUserPreferenceDoubleValue**(swUserPreferenceRoutingDouble\_e.swSlackPercentage))
        Debug.Print("Text size for connection and route points: " & routingSettings.**GetRoutingUserPreferenceDoubleValue**(swUserPreferenceRoutingDouble\_e.swTextSizeForConnectionAndRoutePoints))
        Debug.Print("Rotation increment in degrees: " & routingSettings.**GetRoutingUserPreferenceIntegerValue**(swUserPreferenceRoutingInteger\_e.swComponentRotationIncrementDegrees))
        Debug.Print("Enable minimum bend radius checks: " & routingSettings.**GetRoutingUserPreferenceIntegerValue**(swUserPreferenceRoutingInteger\_e.swEnableMinimumBendRadiusChecks))
        Debug.Print("")
        Debug.Print("Default file locations")
        Debug.Print("  Assembly template: " & routingSettings.**GetRoutingUserPreferenceStringValue**(swUserPreferenceRoutingFileLocations\_e.swFileLocationsRoutingAssemblyTemplate, True))
        Debug.Print("  Cable library: " & routingSettings.**GetRoutingUserPreferenceStringValue**(swUserPreferenceRoutingFileLocations\_e.swFileLocationsRoutingCableLibrary, True))
        Debug.Print("  Component library: " & routingSettings.**GetRoutingUserPreferenceStringValue**(swUserPreferenceRoutingFileLocations\_e.swFileLocationsRoutingComponentLibrary, True))
        Debug.Print("  Covering library: " & routingSettings.**GetRoutingUserPreferenceStringValue**(swUserPreferenceRoutingFileLocations\_e.swFileLocationsRoutingCoveringLibrary, True))
        Debug.Print("  Interconnects library: " & routingSettings.**GetRoutingUserPreferenceStringValue**(swUserPreferenceRoutingFileLocations\_e.swFileLocationsRoutingInterconnectsLibrary, True))
        Debug.Print("  Pipe tube covering library: " & routingSettings.**GetRoutingUserPreferenceStringValue**(swUserPreferenceRoutingFileLocations\_e.swFileLocationsRoutingPipeTubeCoveringLibrary, True))
        Debug.Print("  Standard cable: " & routingSettings.**GetRoutingUserPreferenceStringValue**(swUserPreferenceRoutingFileLocations\_e.swFileLocationsRoutingStandardCable, True))
        Debug.Print("  Standard tubes: " & routingSettings.**GetRoutingUserPreferenceStringValue**(swUserPreferenceRoutingFileLocations\_e.swFileLocationsRoutingStandardTubes, True))
        Debug.Print("  Tag schemes: " & routingSettings.**GetRoutingUserPreferenceStringValue**(swUserPreferenceRoutingFileLocations\_e.swFileLocationsRoutingTagSchemes, True))
        Debug.Print("  Routing library path: " & routingSettings.**GetRoutingUserPreferenceStringValue**(swUserPreferenceRoutingFileLocations\_e.swRoutingLibraryPath, True))
        Debug.Print("")
        Debug.Print("Always use default document template? " & routingSettings.**GetRoutingUserPreferenceToggle**(swUserPreferenceRoutingToggle\_e.swAlwaysUseDefaultDocumentTemplate))
        Debug.Print("Automatically add dimensions to route stubs? " & routingSettings.**GetRoutingUserPreferenceToggle**(swUserPreferenceRoutingToggle\_e.swAutomaticallyAddDimensionToRouteStubs))
        Debug.Print("Automatically create sketch fillets? " & routingSettings.**GetRoutingUserPreferenceToggle**(swUserPreferenceRoutingToggle\_e.swAutomaticallyCreateSketchFillets))
        Debug.Print("Automatically route on drop of clips? " & routingSettings.**GetRoutingUserPreferenceToggle**(swUserPreferenceRoutingToggle\_e.swAutomaticallyRouteOnDropOfClips))
        Debug.Print("Automatically route on drop of flange connectors? " & routingSettings.**GetRoutingUserPreferenceToggle**(swUserPreferenceRoutingToggle\_e.swAutomaticallyRouteOnDropOfFlangeConnectors))
        Debug.Print("Create custom fittings? " & routingSettings.**GetRoutingUserPreferenceToggle**(swUserPreferenceRoutingToggle\_e.swCreateCustomFittings))
        Debug.Print("Create pipes on open line segments? " & routingSettings.**GetRoutingUserPreferenceToggle**(swUserPreferenceRoutingToggle\_e.swCreatePipesOnOpenLineSegments))
        Debug.Print("Display error balloons? " & routingSettings.**GetRoutingUserPreferenceToggle**(swUserPreferenceRoutingToggle\_e.swDisplayErrorBalloons))
        Debug.Print("Enable route error checking? " & routingSettings.**GetRoutingUserPreferenceToggle**(swUserPreferenceRoutingToggle\_e.swEnableRouteErrorChecking))
        Debug.Print("Include coverings in bills of material? " & routingSettings.**GetRoutingUserPreferenceToggle**(swUserPreferenceRoutingToggle\_e.swIncludeCoveringsInBOM))
        Debug.Print("Save route assembly externally? " & routingSettings.**GetRoutingUserPreferenceToggle**(swUserPreferenceRoutingToggle\_e.swSaveRouteAssemblyExternally))
        Debug.Print("Save route parts externally? " & routingSettings.**GetRoutingUserPreferenceToggle**(swUserPreferenceRoutingToggle\_e.swSaveRoutePartsExternally))
        Debug.Print("Use automatic naming for route parts? " & routingSettings.**GetRoutingUserPreferenceToggle**(swUserPreferenceRoutingToggle\_e.swUseAutomaticNamingForRouteParts))
        Debug.Print("User centerline dimension? " & routingSettings.**GetRoutingUserPreferenceToggle**(swUserPreferenceRoutingToggle\_e.swUseCenterlineDim))
        Debug.Print("Use triad to position and orient components? " & routingSettings.**GetRoutingUserPreferenceToggle**(swUserPreferenceRoutingToggle\_e.swUseTriadToPosAndOrientComp))

    End Sub

    ''' <summary>
    ''' The SldWorks swApp variable is pre-assigned for you.
    ''' </summary>
    Public swApp As SldWorks

End Class