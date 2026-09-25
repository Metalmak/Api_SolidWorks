<!-- source: sldworksapi/Rebuild_an_Assembly_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Rebuild an Assembly Example (VB.NET)

This example shows how to rebuild an assembly.

'----------------------------------------------------------------------------
' Preconditions: Open *public\_documents***\samples\tutorial\api\wrench.sldasm**.
'
' Postconditions:
' 1. Rebuilds the assembly.
' 2. Inspect the Immediate window for the result code.
'
' NOTE: Because the model is used elsewhere,
' do not save changes when closing it.
'
---------------------------------------------------------------------------
Imports
SolidWorks.Interop.sldworks
Imports
SolidWorks.Interop.swconst
Imports
System.Runtime.InteropServices
Imports
System
Imports
System.Diagnostics

Partial
Class
SolidWorksMacro

    Dim
part As
ModelDoc2
    Dim
modelDocExt As
ModelDocExtension
    Dim ret
As
Boolean

    Sub
main()

        part = swApp.**ActiveDoc**
        modelDocExt = part.**Extension**
        ret = modelDocExt.**Rebuild**(swRebuildOptions\_e.swRebuildAll)

        Debug.Print("Successfully
rebuilt? " & ret)

    End
Sub

    Public
swApp As
SldWorks

End
Class