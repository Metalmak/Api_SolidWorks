<!-- source: swscanto3dapi/Get_Mesh_Data_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Get Mesh Data Example (C#)

This example shows how to get the mesh feature data from a **\*.3DS** file.
You must have a SOLIDWORKS Premium license to run this example.

//----------------------------------------------------------------------------

// Preconditions:

// 1. Click **Tools > Add-ins > Scanto3D** to activate the
Scanto3D add-in.

// 2. Open a **\*.3DS** file.

// 3. Open an Immediate window.

//

// Postconditions: Inspect the Immediate window.

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

 SolidWorks.Interop.swscanto3d;

using

 System.Runtime.InteropServices;

namespace

 GetMeshData\_CSharp.csproj

{

partial
class
SolidWorksMacro

{

ModelDoc2 swModel;
ModelDocExtension swModelDocExtension;
Scanto3D swScanto3D;
bool boolStatus;
public void
Main()

    {

>     swModel = (

ModelDoc2)swApp.**ActiveDoc**;

    swModelDocExtension = swModel.**Extension**;

    swScanto3D = (

Scanto3D)swModelDocExtension.**GetScanto3D**();
int MeshCount = 0;
int i = 0;
int PointsCount = 0;
int FacetsCount = 0;
object Points =
null;
object Facets =
null;

    MeshCount = swScanto3D.**GetMeshCount**();

Debug.Print("Number
of mesh features: " + MeshCount);
for (i = 0; i <= MeshCount; i++)

    {

>     boolStatus = swScanto3D.**GetMeshDataCountAtIndex**(i,

out
PointsCount, out
FacetsCount);
Debug.Print("Number
of vertexes in mesh feature " + i +
": " +
PointsCount);
Debug.Print("Number
of facets in mesh feature " + i +
": " +
FacetsCount);

    boolStatus = swScanto3D.**GetMeshDataAtIndex**(i,

out
Points, out
Facets);

    }

}

public
SldWorks
swApp;

}

}