<!-- source: swscanto3dapi/Get_Mesh_Data_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Get Mesh Data Example (VB.NET)

This example shows how to get the mesh feature data from a **\*.3DS** file.
You must have a SOLIDWORKS Premium license to run this example.

'----------------------------------------------------------------------------

' Preconditions:

' 1. Click **Tools > Add-ins > Scanto3D** to activate the
Scanto3D add-in.

' 2. Open a **\*.3DS** file.

' 3. Open an Immediate window.

'

' Postconditions: Inspect the Immediate window.

'
---------------------------------------------------------------------------

Imports

 SolidWorks.Interop.sldworks

Imports

 SolidWorks.Interop.swconst

Imports

 SolidWorks.Interop.swscanto3d

Imports

 System.Runtime.InteropServices

Imports

 System

Imports

 System.Diagnostics

Partial

Class SolidWorksMacro
Dim
swModel As
ModelDoc2Dim
swModelDocExtension As
ModelDocExtensionDim
swScanto3D As
Scanto3DDim
boolStatus As
Boolean
Sub
Main()
> swModel = swApp.**ActiveDoc**
>
> swModelDocExtension = swModel.**Extension**
>
> swScanto3D = swModelDocExtension.**GetScanto3D**()

Dim
MeshCount As
Integer
Dim
i As
Integer
Dim
PointsCount As
Integer
Dim
FacetsCount As
Integer
Dim
Points As
Object =
Nothing
Dim
Facets As
Object =
Nothing

MeshCount = swScanto3D.**GetMeshCount**()

Debug.Print(

"Number
of mesh features: " & MeshCount)For
i = 0 To
MeshCount
> boolStatus = swScanto3D.**GetMeshDataCountAtIndex**(i,
> PointsCount, FacetsCount)
>
> Debug.Print(

"Number
of vertexes in mesh feature " & i &
": " &
PointsCount)

Debug.Print(

"Number
of facets in mesh feature " & i &
": " &
FacetsCount)

boolStatus = swScanto3D.**GetMeshDataAtIndex**(i,
Points, Facets)

Next

End
SubPublic
swApp As
SldWorks

End

Class