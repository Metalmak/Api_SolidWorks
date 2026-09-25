<!-- source: sldworksapi/Save_File_Example_VB.htm -->

# SOLIDWORKS API Help

# Save File Example (VBA)

This example shows how to save a file.

```
'-----------------------------------------------------------------
' Preconditions:
' 1. Open a model.
' 2. Open the Immediate window.
'
' Postconditions:
' 1. Zooms to fit the model in the graphics area.
' 2. Saves the model.
' 3. Examine the graphics area and Immediate window.
'------------------------------------------------------------------
Option Explicit
```

    Dim swApp
As SldWorks.SldWorks
    Dim swModel
As SldWorks.ModelDoc2
    Dim boolstatus
As Boolean
    Dim lErrors
As Long
    Dim lWarnings
As Long

Sub main()

    Set swApp = Application.**SldWorks**
    Set swModel = swApp.**ActiveDoc**
    swApp.**Visible** = True

    ' Make a change
    swModel.**ViewZoomtofit2**

    boolstatus = swModel.**Save3**(swSaveAsOptions\_Silent,
lErrors, lWarnings)

    ' Errors
    Debug.Print ("Errors as defined in swFileSaveError\_e: " &
lErrors)

    ' Warnings
    Debug.Print ("Warnings as defined in swFileSaveWarning\_e: " &
lWarnings)

End Sub