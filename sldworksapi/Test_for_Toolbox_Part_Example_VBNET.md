<!-- source: sldworksapi/Test_for_Toolbox_Part_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Test for Toolbox Part Example (VB.NET)

This example shows how to test whether a part is a Toolbox part.

'----------------------------------------------------------------------------
' Preconditions: Open *public\_documents***\samples\tutorial\api\bagel.sldprt**.
'
' Postconditions: Inspect the Immediate window for the Toolbox part type.
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
Integer

    Sub
main()

        part = swApp.**ActiveDoc**
        modelDocExt = part.**Extension**
        ret = modelDocExt.**ToolboxPartType**

        Debug.Print("Toolbox part type as
defined in swToolBoxPartType\_e? " & ret)

    End
Sub

    Public
swApp As
SldWorks

End
Class