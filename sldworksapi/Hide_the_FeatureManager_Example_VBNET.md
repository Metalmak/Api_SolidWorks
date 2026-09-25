<!-- source: sldworksapi/Hide_the_FeatureManager_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Hide the FeatureManager Design Tree Example (VB.NET)

This example shows how to hide the FeatureManager design tree.

'------------------------------------------------------
' Preconditions: Open a model document.
'
' Postconditions:
' 1. Hides the FeatureManager design tree.
' 2. Examine SOLIDWORKS.
'------------------------------------------------------

Imports
SolidWorks.Interop.sldworks
Imports
SolidWorks.Interop.swconst
Imports
System

Partial
Class
SolidWorksMacro

    Sub
main()

        Dim
swModel As
ModelDoc2
        Dim
swModDocExt As
ModelDocExtension
        Dim
bRet As
Boolean

        swModel = swApp.**ActiveDoc**
        swModDocExt = swModel.**Extension**
        bRet = swModDocExt.**HideFeatureManager**(True)
    End
Sub

    Public
swApp As
SldWorks

End
Class