<!-- source: sldworksapi/Get_and_Set_User_Preferences_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Get and Set User Preferences Example (C#)

This sample code demonstrates how to use the methods for getting and setting various system options and document properties.

//--------------------------------------------------------------------------
// Preconditions:
//  1.
Open a
drawing document.
//  2.
Create
a layer named **test** in the drawing.
//  3.
Open an
Immediate window.
//
// Postconditions:
// 1.
Observe
the new settings in the Immediate window.
// 2. Maps the value returned by the GetUserPreferenceInteger
//    method to the corresponding enumerator member in the enumerator

//    online
help.
// 3. Click **Tools > Options** in SOLIDWORKS and verify the new settings.
//-------------------------------------------------------------------------

using SolidWorks.Interop.sldworks;

using SolidWorks.Interop.swconst;

using System;

using System.Diagnostics;

namespace UserPreferences\_CSharp.csproj

{

partial class SolidWorksMacro

{

    public
SldWorks swApp;

    public
void Main()

    {

        ModelDoc2
Part = null;

        bool
boolstatus = false;

        TextFormat
swTextFormat = default(TextFormat);

        object
TextFormatObj = null;

        ModelDocExtension
ModelDocExtension = default(ModelDocExtension);

        Part
= (ModelDoc2)swApp.**ActiveDoc**;

        ModelDocExtension
= Part.**Extension**;

        //The
following call demonstrates how to get and set a Tools > Options
> System Options > General option

        //Custom
property used as component description

        boolstatus
= swApp.SetUserPreferenceStringValue((int)swUserPreferenceStringValue\_e.swCustomPropertyUsedAsComponentDescription,
"Status");

        Debug.Print("Tools
> Options > System Options > General > Custom property used
as component description: " + swApp.GetUserPreferenceStringValue((int)swUserPreferenceStringValue\_e.swCustomPropertyUsedAsComponentDescription));

        //The
following calls demonstrate how to get and set Tools > Options
> System Options > View options

        //Reverse
mouse wheel zoom direction

        swApp.SetUserPreferenceToggle((int)swUserPreferenceToggle\_e.swViewReverseWheelZoomDirection,
true);

        Debug.Print("Tools
> Options > System Options > View > Reverse mouse wheel zoom
direction: " + swApp.GetUserPreferenceToggle((int)swUserPreferenceToggle\_e.swViewReverseWheelZoomDirection));

        //View
rotation - Arrow keys

        boolstatus
= swApp.SetUserPreferenceDoubleValue((int)swUserPreferenceDoubleValue\_e.swViewRotationArrowKeys,
0.2268928027593);

        //1 radian = 180º/p
= 57.295779513º or approximately 57.3º

        Debug.Print("Tools
> Options > System Options > View > Arrow keys: " + swApp.GetUserPreferenceDoubleValue((int)swUserPreferenceDoubleValue\_e.swViewRotationArrowKeys)
\* 57.3);

        //Convert
to degrees

        //View
rotation - Mouse speed

        boolstatus
= swApp.SetUserPreferenceIntegerValue((int)swUserPreferenceIntegerValue\_e.swViewRotationMouseSpeed,
56);

        Debug.Print("Tools
> Options > System Options > View > Mouse speed: " +
swApp.GetUserPreferenceIntegerValue((int)swUserPreferenceIntegerValue\_e.swViewRotationMouseSpeed));

        //Transitions
- View transition

        boolstatus
= swApp.SetUserPreferenceDoubleValue((int)swUserPreferenceDoubleValue\_e.swViewAnimationSpeed,
2.5);

        Debug.Print("Tools
> Options > System Options > View > View transition: "
+ swApp.GetUserPreferenceDoubleValue((int)swUserPreferenceDoubleValue\_e.swViewAnimationSpeed));

        //Transitions
- Hide/show component

        boolstatus
= swApp.SetUserPreferenceDoubleValue((int)swUserPreferenceDoubleValue\_e.swViewTransitionHideShowComponent,
0.8000000119209);

        Debug.Print("Tools
> Options > System Options > View > Hide/show component: "
+ swApp.GetUserPreferenceDoubleValue((int)swUserPreferenceDoubleValue\_e.swViewTransitionHideShowComponent));

        //Transitions
- Isolate

        boolstatus
= swApp.SetUserPreferenceDoubleValue((int)swUserPreferenceDoubleValue\_e.swViewTransitionIsolate,
1.222222208977);

        Debug.Print("Tools
> Options > System Options > View > Isolate: " + swApp.GetUserPreferenceDoubleValue((int)swUserPreferenceDoubleValue\_e.swViewTransitionIsolate));

        //The
following calls demonstrate how to get and set the Tools > Options
> Document Properties > Drafting Standard option

        //Maps the value returned by the GetUserPreferenceInteger
method to the corresponding enumerator member in the enumerator online help

        //Overall
drafting standard

        boolstatus
= ModelDocExtension.SetUserPreferenceInteger((int)swUserPreferenceIntegerValue\_e.swDetailingDimensionStandard,
(int)swUserPreferenceOption\_e.swDetailingNoOptionSpecified, (int)swDetailingStandard\_e.swDetailingStandardISO);

        string
sText = null;

        sText
= "Tools > Options > Document Properties > Drafting Standard
> Overall drafting standard is ";

        switch
(ModelDocExtension.GetUserPreferenceInteger((int)swUserPreferenceIntegerValue\_e.swDetailingDimensionStandard,
(int)swUserPreferenceOption\_e.swDetailingNoOptionSpecified))

        {

            case
1:

                Debug.Print(sText
+ "ANSI");

                break;

            case
2:

                Debug.Print(sText
+ "ISO");

                break;

            case
3:

                Debug.Print(sText
+ "DIN");

                break;

            case
4:

                Debug.Print(sText
+ "JIS");

                break;

            case
5:

                Debug.Print(sText
+ "BS");

                break;

            case
6:

                Debug.Print(sText
+ "GOST");

                break;

            case
7:

                Debug.Print(sText
+ "GB");

                break;

            case
8:

                Debug.Print(sText
+ "User Defined");

                break;

        }

        //The
following calls demonstrate how to get and set Tools > Options > Document
Properties > Annotations > Balloons options

        //Maps the value returned by the GetUserPreferenceInteger
method to the corresponding enumerator member in the enumerator online help

        //Leader
style - Leader Thickness

        boolstatus
= ModelDocExtension.SetUserPreferenceInteger((int)swUserPreferenceIntegerValue\_e.swDetailingBalloonLeaderLineThickness,
0, (int)swLineWeights\_e.swLW\_NUMBER);

        Debug.Print("Tools
> Options > Document Properties > Annotations > Balloons >
Leader Thickness: " + ModelDocExtension.GetUserPreferenceInteger((int)swUserPreferenceIntegerValue\_e.swDetailingBalloonLeaderLineThickness,
0));

        //Leader
style - Custom leader thickness

        boolstatus
= ModelDocExtension.SetUserPreferenceDouble((int)swUserPreferenceDoubleValue\_e.swDetailingBalloonLeaderLineThicknessCustom,
0, 0.00028);

        Debug.Print("Tools
> Options > Document Properties > Annotations > Balloons >
Custom Leader Thickness: " + ModelDocExtension.GetUserPreferenceDouble((int)swUserPreferenceDoubleValue\_e.swDetailingBalloonLeaderLineThicknessCustom,
0));

        //Frame
style - Frame Thickness

        boolstatus
= ModelDocExtension.SetUserPreferenceInteger((int)swUserPreferenceIntegerValue\_e.swDetailingBalloonFrameLineThickness,
0, (int)swLineWeights\_e.swLW\_NUMBER);

        Debug.Print("Tools
> Options > Document Properties > Annotations > Balloons >
Frame Thickness: " + ModelDocExtension.GetUserPreferenceInteger((int)swUserPreferenceIntegerValue\_e.swDetailingBalloonFrameLineThickness,
0));

        //Frame
style - Custom frame thickness

        boolstatus
= ModelDocExtension.SetUserPreferenceDouble((int)swUserPreferenceDoubleValue\_e.swDetailingBalloonFrameLineThicknessCustom,
0, 0.00028);

        Debug.Print("Tools
> Options > Document Properties > Annotations > Balloons >
Custom Frame Thickness: " + ModelDocExtension.GetUserPreferenceDouble((int)swUserPreferenceDoubleValue\_e.swDetailingBalloonFrameLineThicknessCustom,
0));

        //Text
- Upper - Custom property

        boolstatus
= ModelDocExtension.SetUserPreferenceString((int)swUserPreferenceStringValue\_e.swDetailingBOMUpperCustomProperty,
0, "Source");

        Debug.Print("Tools
> Options > Document Properties > Annotations > Balloons >
Text Upper Custom property: " + ModelDocExtension.GetUserPreferenceString((int)swUserPreferenceStringValue\_e.swDetailingBOMUpperCustomProperty,
0));

        //Single
balloon - Style

        boolstatus
= ModelDocExtension.SetUserPreferenceInteger((int)swUserPreferenceIntegerValue\_e.swDetailingBOMBalloonStyle,
0, (int)swBalloonStyle\_e.swBS\_Triangle);

        Debug.Print("Tools
> Options > Document Properties > Annotations > Balloons >
Single balloon - Style: " + ModelDocExtension.GetUserPreferenceInteger((int)swUserPreferenceIntegerValue\_e.swDetailingBOMBalloonStyle,
0));

        //Single
balloon - Size

        boolstatus
= ModelDocExtension.SetUserPreferenceInteger((int)swUserPreferenceIntegerValue\_e.swDetailingBOMBalloonFit,
0, (int)swBalloonFit\_e.swBF\_3Chars);

        Debug.Print("Tools
> Options > Document Properties > Annotations > Balloons >
Single balloon - Size: " + ModelDocExtension.GetUserPreferenceInteger((int)swUserPreferenceIntegerValue\_e.swDetailingBOMBalloonFit,
0));

        //Stacked
balloons - Style

        boolstatus
= ModelDocExtension.SetUserPreferenceInteger((int)swUserPreferenceIntegerValue\_e.swDetailingBOMStackedBalloonStyle,
0, (int)swBalloonStyle\_e.swBS\_Triangle);

        Debug.Print("Tools
> Options > Document Properties > Annotations > Balloons >
Stacked balloons - Style: " + ModelDocExtension.GetUserPreferenceInteger((int)swUserPreferenceIntegerValue\_e.swDetailingBOMStackedBalloonStyle,
0));

        //Stacked
balloons - Size

        boolstatus
= ModelDocExtension.SetUserPreferenceInteger((int)swUserPreferenceIntegerValue\_e.swDetailingBOMStackedBalloonFit,
0, (int)swBalloonFit\_e.swBF\_3Chars);

        Debug.Print("Tools
> Options > Document Properties > Annotations > Balloons >
Stacked balloons - Size: " + ModelDocExtension.GetUserPreferenceInteger((int)swUserPreferenceIntegerValue\_e.swDetailingBOMStackedBalloonFit,
0));

        //Auto
balloon layout

        boolstatus
= ModelDocExtension.SetUserPreferenceInteger((int)swUserPreferenceIntegerValue\_e.swDetailingAutoBalloonLayout,
0, (int)swBalloonLayoutType\_e.swDetailingBalloonLayout\_Right);

        Debug.Print("Tools
> Options > Document Properties > Annotations > Balloons >
Auto balloon layout: " + ModelDocExtension.GetUserPreferenceInteger((int)swUserPreferenceIntegerValue\_e.swDetailingAutoBalloonLayout,
0));

        //Leader
display - Use document leader length

        boolstatus
= ModelDocExtension.SetUserPreferenceToggle((int)swUserPreferenceToggle\_e.swDetailingBalloonUseDocBentLeaderLength,
0, true);

        Debug.Print("Tools
> Options > Document Properties > Annotations > Balloons >
Leader display - Use document leader length: " + ModelDocExtension.GetUserPreferenceToggle((int)swUserPreferenceToggle\_e.swDetailingBalloonUseDocBentLeaderLength,
0));

        //Layer

        boolstatus
= ModelDocExtension.SetUserPreferenceString((int)swUserPreferenceStringValue\_e.swDetailingLayer,
(int)swUserPreferenceOption\_e.swDetailingBalloon, "test");

        Debug.Print("Tools
> Options > Document Properties > Annotations > Balloons >
Layer: " + ModelDocExtension.GetUserPreferenceString((int)swUserPreferenceStringValue\_e.swDetailingLayer,
(int)swUserPreferenceOption\_e.swDetailingBalloon));

        //Font

        TextFormatObj
= ModelDocExtension.GetUserPreferenceTextFormat((int)swUserPreferenceTextFormat\_e.swDetailingBalloonTextFormat,
0);

        swTextFormat
= (TextFormat)TextFormatObj;

        swTextFormat.Italic
= true;

        swTextFormat.Bold
= true;

        boolstatus
= ModelDocExtension.SetUserPreferenceTextFormat((int)swUserPreferenceTextFormat\_e.swDetailingBalloonTextFormat,
0, swTextFormat);

        Debug.Print("Tools
> Options > Document Properties > Annotations > Balloons >
Font is italic and bold: " + boolstatus);

    }

}

}