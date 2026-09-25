<!-- source: sldworksapi/Get_and_Set_Sunlight_Source_Property_Values_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Get and Set Sunlight Source Property Values Example (C#)

This example shows how to get and set sunlight properties.

//----------------------------------------------------------------------------

// Preconditions:

// 1. Open a part with a sunlight source.

// 2. Open an Immediate window.

//

// Postconditions: Inspect the Immediate window for the
sunlight properties.

//
---------------------------------------------------------------------------

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

SunlightProperties\_CSharp.csproj

{

partial
class
SolidWorksMacro

{

ModelDoc2
swModelDoc;
ModelDocExtension swModelDocExt;bool
retval;MathVector
NorthDirection;string
DateTime;object
vVector;double[]
nVector = new
double[3];MathUtility
swMathUtil;double
NorthLatitude;double
EastLongitude;double
TimeZone;double
Haze;double
SunDiameter;int
GroundAlbedo;double
SkyGamma;public
void Main()

{

> swModelDoc = (

ModelDoc2)swApp.**ActiveDoc**;

swModelDocExt = swModelDoc.**Extension**;

//Get
sunlight properties

retval = swModelDocExt.**GetSunLightSourcePropertyValues**(

out
NorthDirection, out
NorthLatitude, out
EastLongitude, out
TimeZone, out
DateTime);

retval = swModelDocExt.**GetSunLightAdvancedPropertyValues**(

out
Haze, out
SunDiameter, out
GroundAlbedo, out
SkyGamma);Debug.Print("North
direction: " + ((double[])(NorthDirection.**ArrayData**))[0]
+ "," +
((double[])(NorthDirection.**ArrayData**))[1]
+ "," +
((double[])(NorthDirection.**ArrayData**))[2]);Debug.Print("North
latitude:
" + NorthLatitude);Debug.Print("East
longitude:
" + EastLongitude);Debug.Print("Time
zone:
" + TimeZone);Debug.Print("Date
and time:
" + DateTime);Debug.Print("Haze
(0.0 - 1.0): " + Haze);Debug.Print("Sun
diameter (0.01 - 21474836.47): " + SunDiameter);Debug.Print("RGB
for ground albedo: " + GroundAlbedo);Debug.Print("Sky
Gamma (0.1 = 100.0): " + SkyGamma);

Debug.Print("Minutes
of sunlight: " + swModelDocExt.**get\_SunLightInformation**((int)swSunlightInfoType\_e.swSunlight\_LengthOfDay**));**

Debug.Print("Sunrise
(hours from midnight): " + swModelDocExt.**get\_SunLightInformation**((int)swSunlightInfoType\_e.swSunlight\_Sunrise));

Debug.Print("Sunset
(hours from midnight): " + swModelDocExt.**get\_SunLightInformation**((int)swSunlightInfoType\_e.swSunlight\_Sunset));

//Set
sunlight source property values

swMathUtil = (

MathUtility)swApp.**GetMathUtility**();

nVector[0] = 1;

nVector[1] = 0;

nVector[2] = 0;

vVector = nVector;

NorthDirection = (

MathVector)swMathUtil.**CreateVector**((vVector));

DateTime =

"11/9/2012 2:48:13 PM";

NorthLatitude = NorthLatitude + 0.1;

EastLongitude = EastLongitude + 0.1;

TimeZone = TimeZone + 0.5;

retval = swModelDocExt.**SetSunLightSourcePropertyValues**(NorthDirection,
NorthLatitude, EastLongitude, TimeZone, DateTime);

}

public SldWorks
swApp;

}

}