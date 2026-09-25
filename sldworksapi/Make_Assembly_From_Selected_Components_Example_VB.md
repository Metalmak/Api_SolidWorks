<!-- source: sldworksapi/Make_Assembly_From_Selected_Components_Example_VB.htm -->

# SOLIDWORKS API Help

# Make Assembly From Selected Components Example (VBA)

This example shows how to create a new assembly using the selected components
of the active assembly.

'---------------------------------------------------------------------
' Preconditions:
' 1. Open *public\_documents***\samples\tutorial\motionstudies\valve\_cam2.sldasm**
' 2. Ensure that the **Save new components to external files** check box
'    on the **Tools > Options > Assemblies** dialog is
selected.
'    Otherwise, the selected components are saved as virtual
components
'    and not as external files.
' 3. Select **valve<1>** and **valve\_guide<1>** components.
'
' Postconditions:
' 1. Creates *public\_documents***\samples\tutorial\motionstudies\MyTestValveAssembly.sldasm**,

'    which is made up of the **valve<1>** and **valve\_guide<1>**components.
' 2. Replaces the **valve<1>** and **valve\_guide<1>** components with
'    **MyTestValveAssembly** subassembly.
' 3. Examine the FeatureManager design tree and
'    *public\_documents***\samples\tutorial\motionstudies**.
' 4. Clear the S**ave new components to external files** check box
'    on the **Tools > Options > Assemblies** dialog if you
selected
'    it for this example.
'
' NOTE: Because the assembly is used elsewhere, do not save changes.
'-----------------------------------------------------------------------

Option Explicit

Dim swApp As SldWorks.SldWorks

Dim swModel As SldWorks.ModelDoc2

Dim swAssy As SldWorks.AssemblyDoc

Dim tmpPath As String

Dim boolstat As Boolean

Sub main()

    Set
swApp = Application.SldWorks

    Set
swModel = swApp.ActiveDoc

    boolstat
= True

    Dim
strCompModelname As String

    strCompModelname
= "MyTestValveAssembly.sldasm"

    '
Save the new assembly in the same folder as the original assembly

    tmpPath
= Left(swModel.GetPathName, InStrRev(swModel.GetPathName, "\"))

    Set
swAssy = swModel

    '
Create a new assembly using the selected components

    swAssy.MakeAssemblyFromSelectedComponents (tmpPath
+ strCompModelname)

End Sub