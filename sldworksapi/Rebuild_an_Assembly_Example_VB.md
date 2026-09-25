<!-- source: sldworksapi/Rebuild_an_Assembly_Example_VB.htm -->

# SOLIDWORKS API Help

# Rebuild an Assembly Example (VBA)

This example shows how to rebuild an assembly.

'----------------------------------------------------------------------------
' Preconditions: Open *public\_documents***\samples\tutorial\api\wrench.sldasm**.
'
' Postconditions:
' 1. Rebuilds the assembly.
' 2. Inspect the Immediate window for the result code.
'
' NOTE: Because the model is used elsewhere, do not save changes.
' ---------------------------------------------------------------------------

Dim swApp As SldWorks.SldWorks
Dim part As SldWorks.ModelDoc2
Dim modelDocExt As SldWorks.ModelDocExtension
Dim ret As Boolean

Option Explicit
Sub main()

    Set swApp = Application.**SldWorks**
    Set part = swApp.**ActiveDoc**
    Set modelDocExt = part.**Extension**
    ret = modelDocExt.**Rebuild**(swRebuildOptions\_e.swRebuildAll)

    Debug.Print "Successfully rebuilt? " & ret

End Sub