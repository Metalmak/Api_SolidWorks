<!-- source: sldworksapi/Get_Whether_Feature_is_Locked_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Get Whether Feature is Frozen Example (VB.NET)

This example shows how to get whether a feature is frozen.

'---------------------------------------------------------------------------
' Preconditions:
' 1. Open a part or assembly.
' 2. Select a frozen feature in the FeatureManager design tree.
'
' Postconditions: Inspect the Immediate Window.
'-----------------------------------------------

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

    Sub
main()

        Dim
swModel As
ModelDoc2
        Dim
swSelMgr As
SelectionMgr
        Dim
swFeat As
Feature
        Dim
bRet As
Boolean

        swModel = swApp.ActiveDoc
        swSelMgr = swModel.SelectionManager
        swFeat = swSelMgr.GetSelectedObject6(1, -1)

        bRet = swFeat.**IsFrozen**
        Debug.Print("Feature is
frozen? "
& bRet)

    End
Sub

    Public
swApp As
SldWorks

End
Class