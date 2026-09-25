<!-- source: sldworksapi/Get_and_Set_User_Preferences_Example_VB.htm -->

# SOLIDWORKS API Help

# Get and Set User Preferences Example (VBA)

This sample code demonstrates how to get and set
various system options and document properties.

'---------------------------------------------------------------------------
' Preconditions:
' 1.
 Open a
drawing document.
' 2.
 Create a layer
named **test** in the document.
' 3.
 Open an
Immediate window.
'
' Postconditions:
' 1. Observe
the new settings in the Immediate window.
' 2. Maps the value returned by the GetUserPreferenceInteger
method
'    to the corresponding enumerator member in the enumerator online
help.
' 3. Click **Tools > Options** in SOLIDWORKS and verify the new settings.
'----------------------------------------------------------------------------

Dim swApp As Object

Dim Part As Object

Dim boolstatus As Boolean

Dim longstatus As Long, longwarnings As Long

Dim swTextFormat As SldWorks.TextFormat

Dim TextFormatObj As Object

Dim ModelDocExtension As ModelDocExtension

Sub main()

Set swApp = Application.SldWorks

Set Part = swApp.**ActiveDoc**

Set ModelDocExtension = Part.**Extension**

    'The following call demonstrates how to get and set
a Tools > Options > System Options > General option

    'Custom
property used as component description

    boolstatus
= swApp.SetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swCustomPropertyUsedAsComponentDescription,
"Status")

    Debug.Print
"Tools > Options > System Options > General > Custom
property used as component description: " & swApp.GetUserPreferenceStringValue(swUserPreferenceStringValue\_e.swCustomPropertyUsedAsComponentDescription)

    'The following calls demonstrate how to get and set
Tools > Options > System Options > View options

    'Reverse
mouse wheel zoom direction

    swApp.SetUserPreferenceToggle swUserPreferenceToggle\_e.swViewReverseWheelZoomDirection,
True

    Debug.Print
"Tools > Options > System Options > View > Reverse mouse
wheel zoom direction: " & swApp.GetUserPreferenceToggle(swUserPreferenceToggle\_e.swViewReverseWheelZoomDirection)

    'View
rotation - Arrow keys

    boolstatus
= swApp.SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swViewRotationArrowKeys,
0.2268928027593)

    '1 radian = 180º/p
= 57.295779513º or approximately 57.3º

    Debug.Print
"Tools > Options > System Options > View > Arrow keys:
" & swApp.GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swViewRotationArrowKeys)
\* 57.3 'Convert to degrees

    'View
rotation - Mouse speed

    boolstatus
= swApp.SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swViewRotationMouseSpeed,
56)

    Debug.Print
"Tools > Options > System Options > View > Mouse speed:
" & swApp.GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swViewRotationMouseSpeed)

    'Transitions
- View transition

    boolstatus
= swApp.SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swViewAnimationSpeed,
2.5)

    Debug.Print
"Tools > Options > System Options > View > View transition:
" & swApp.GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swViewAnimationSpeed)

    'Transitions
- Hide/show component

    boolstatus
= swApp.SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swViewTransitionHideShowComponent,
0.8000000119209)

    Debug.Print
"Tools > Options > System Options > View > Hide/show
component: " & swApp.GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swViewTransitionHideShowComponent)

    'Transitions
- Isolate

    boolstatus
= swApp.SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swViewTransitionIsolate,
1.222222208977)

    Debug.Print
"Tools > Options > System Options > View > Isolate: "
& swApp.GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swViewTransitionIsolate)

    'The following calls demonstrate how to get and set
the Tools > Options > Document Properties > Drafting Standard
option.

    'Map the value returned by the GetUserPreferenceInteger
method to the corresponding enumerator member in the enumerator online help

    'Overall
drafting standard

    boolstatus
= ModelDocExtension.SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingDimensionStandard,
swUserPreferenceOption\_e.swDetailingNoOptionSpecified, swDetailingStandard\_e.swDetailingStandardISO)

    Dim
sText As String

    sText
= "Tools > Options > Document Properties > Drafting Standard
> Overall drafting standard is "

    Select
Case ModelDocExtension.GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingDimensionStandard,
swUserPreferenceOption\_e.swDetailingNoOptionSpecified)

        Case
1

            Debug.Print
sText & "ANSI"

        Case
2

            Debug.Print
sText & "ISO"

        Case
3

            Debug.Print
sText & "DIN"

        Case
4

            Debug.Print
sText & "JIS"

        Case
5

            Debug.Print
sText & "BS"

        Case
6

            Debug.Print
sText & "GOST"

        Case
7

            Debug.Print
sText & "GB"

        Case
8

            Debug.Print
sText & "User Defined"

      End
Select

     'The following API calls demonstrate
how to get and set Tools > Options > Document Properties > Annotations >
Balloons options

     'Map the value returned by the GetUserPreferenceInteger
method to the corresponding enumerator member in the enumerator online help

    'Leader
style - Leader Thickness

    boolstatus
= ModelDocExtension.SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingBalloonLeaderLineThickness,
0, swLineWeights\_e.swLW\_NUMBER)

    Debug.Print
"Tools > Options > Document Properties > Annotations >
Balloons > Leader Thickness: " & ModelDocExtension.GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingBalloonLeaderLineThickness,
0)

    'Leader
style - Custom leader thickness

    boolstatus
= ModelDocExtension.SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDetailingBalloonLeaderLineThicknessCustom,
0, 0.00028)

    Debug.Print
"Tools > Options > Document Properties > Annotations >
Balloons > Custom Leader Thickness: " & ModelDocExtension.GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDetailingBalloonLeaderLineThicknessCustom,
0)

    'Frame
style - Frame Thickness

    boolstatus
= ModelDocExtension.SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingBalloonFrameLineThickness,
0, swLineWeights\_e.swLW\_NUMBER)

    Debug.Print
"Tools > Options > Document Properties > Annotations >
Balloons > Frame Thickness: " & ModelDocExtension.GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingBalloonFrameLineThickness,
0)

    'Frame
style - Custom frame thickness

    boolstatus
= ModelDocExtension.SetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDetailingBalloonFrameLineThicknessCustom,
0, 0.00028)

    Debug.Print
"Tools > Options > Document Properties > Annotations >
Balloons > Custom Frame Thickness: " & ModelDocExtension.GetUserPreferenceDouble(swUserPreferenceDoubleValue\_e.swDetailingBalloonFrameLineThicknessCustom,
0)

    'Text
- Upper - Custom property

    boolstatus
= ModelDocExtension.SetUserPreferenceString(swUserPreferenceStringValue\_e.swDetailingBOMUpperCustomProperty,
0, "Source")

    Debug.Print
"Tools > Options > Document Properties > Annotations >
Balloons > Text Upper Custom property: " & ModelDocExtension.GetUserPreferenceString(swUserPreferenceStringValue\_e.swDetailingBOMUpperCustomProperty,
0)

    'Single
balloon - Style

    boolstatus
= ModelDocExtension.SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingBOMBalloonStyle,
0, swBalloonStyle\_e.swBS\_Triangle)

    Debug.Print
"Tools > Options > Document Properties > Annotations >
Balloons > Single balloon - Style: " & ModelDocExtension.GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingBOMBalloonStyle,
0)

    'Single
balloon - Size

    boolstatus
= ModelDocExtension.SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingBOMBalloonFit,
0, swBalloonFit\_e.swBF\_3Chars)

    Debug.Print
"Tools > Options > Document Properties > Annotations >
Balloons > Single balloon - Size: " & ModelDocExtension.GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingBOMBalloonFit,
0)

    'Stacked
balloons - Style

    boolstatus
= ModelDocExtension.SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingBOMStackedBalloonStyle,
0, swBalloonStyle\_e.swBS\_Triangle)

    Debug.Print
"Tools > Options > Document Properties > Annotations >
Balloons > Stacked balloons - Style: " & ModelDocExtension.GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingBOMStackedBalloonStyle,
0)

    'Stacked
balloons - Size

    boolstatus
= ModelDocExtension.SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingBOMStackedBalloonFit,
0, swBalloonFit\_e.swBF\_3Chars)

    Debug.Print
"Tools > Options > Document Properties > Annotations >
Balloons > Stacked balloons - Size: " & ModelDocExtension.GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingBOMStackedBalloonFit,
0)

    'Auto
balloon layout

    boolstatus
= ModelDocExtension.SetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingAutoBalloonLayout,
0, swBalloonLayoutType\_e.swDetailingBalloonLayout\_Right)

    Debug.Print
"Tools > Options > Document Properties > Annotations >
Balloons > Auto balloon layout: " & ModelDocExtension.GetUserPreferenceInteger(swUserPreferenceIntegerValue\_e.swDetailingAutoBalloonLayout,
0)

    'Leader
display - Use document leader length

    boolstatus
= ModelDocExtension.SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingBalloonUseDocBentLeaderLength,
0, True)

    Debug.Print
"Tools > Options > Document Properties > Annotations >
Balloons > Leader display - Use document leader length: " &
ModelDocExtension.GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDetailingBalloonUseDocBentLeaderLength,
0)

    'Layer

    boolstatus
= ModelDocExtension.SetUserPreferenceString(swUserPreferenceStringValue\_e.swDetailingLayer,
swUserPreferenceOption\_e.swDetailingBalloon, "test")

    Debug.Print
"Tools > Options > Document Properties > Annotations >
Balloons > Layer: " & ModelDocExtension.GetUserPreferenceString(swUserPreferenceStringValue\_e.swDetailingLayer,
swUserPreferenceOption\_e.swDetailingBalloon)

    'Font...

        Set
TextFormatObj = ModelDocExtension.GetUserPreferenceTextFormat(swUserPreferenceTextFormat\_e.swDetailingBalloonTextFormat,
0)

        Set
swTextFormat = TextFormatObj

        swTextFormat.Italic
= True

        swTextFormat.Bold
= True

        boolstatus
= ModelDocExtension.SetUserPreferenceTextFormat(swUserPreferenceTextFormat\_e.swDetailingBalloonTextFormat,
0, swTextFormat)

        Debug.Print
"Tools > Options > Document Properties > Annotations >
Balloons > Font is italic and bold: " & boolstatus

End Sub