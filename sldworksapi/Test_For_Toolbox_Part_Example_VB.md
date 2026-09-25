<!-- source: sldworksapi/Test_For_Toolbox_Part_Example_VB.htm -->

# SOLIDWORKS API Help

# Test for Toolbox Part Example (VBA)

This example shows how to test whether a part is a Toolbox part.

'----------------------------------------------------------------------------
' Preconditions: Open *public\_documents***\samples\tutorial\api\bagel.sldprt.**
'
' Postconditions: Inspect the Immediate window for the Toolbox part type.
'
' NOTE: Because the model is used elsewhere,
' do not save changes when closing it.
' ---------------------------------------------------------------------------

Dim swApp As SldWorks.SldWorks
Dim part As SldWorks.ModelDoc2
Dim modelDocExt As SldWorks.ModelDocExtension
Dim ret As Long

Option Explicit
Sub main()

    Set swApp = Application.**SldWorks**
    Set part = swApp.**ActiveDoc**
    Set modelDocExt = part.**Extension**
    ret = modelDocExt.**ToolboxPartType**

    Debug.Print "Toolbox part type as defined
in swToolBoxPartType\_e? " & ret

End Sub