<!-- source: sldworksapi/Isolate_Changed_Dimension_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Isolate Changed Dimension Example (VB.NET)

This example shows how to isolate a changed dimension.

'------------------------------------------------------
' Preconditions: Verify that the specified drawing and part
' documents exist.
'
' Postconditions:
' 1. Opens the drawing document.
' 2. Sets the system option to display
'    changed dimensions in the color selected
'    for **Tools > Options > System Options >
'    Colors > Color scheme settings >
'    Drawings, Changed dimensions**.
' 3. Saves and closes the drawing document.
' 4. Opens the part document of the drawing document.
' 5. Changes a dimension.
' 6. Saves and closes the part document.
' 7. Opens the previously saved drawing document.
' 8. Examine the drawing document to verify that
'    the changed dimension is displayed in the
'    changed-dimension
color. Place your cursor over
'    the dimension
to see its previous value.
'-------------------------------------------------------
Imports
SolidWorks.Interop.sldworks
Imports
SolidWorks.Interop.swconst
Imports
System

Partial
Class
SolidWorksMacro

    Public
Sub Main()

        Dim
swModel As
ModelDoc2
        Dim
swModelDocExt As
ModelDocExtension
        Dim
swDrawing As
DrawingDoc
        Dim
fileName As
String
        Dim
saveFileName As
String
        Dim
errors As
Long
        Dim
warnings As
Long
        Dim
status As
Boolean

        '
Open drawing document
        fileName =
"C:\Users\Public\Documents\SOLIDWORKS\SOLIDWORKS
2018\samples\tutorial\api\box.slddrw"
        swModel = swApp.**OpenDoc6**(fileName,
swDocumentTypes\_e.swDocDRAWING, swOpenDocOptions\_e.swOpenDocOptions\_Silent,
"",
errors, warnings)

        ' Isolate changed dimensions
        '
Equivalent to selecting Tools > Options > System Options > Colors >

        '
Use specified color for changed drawing dimensions on open
        swApp.**SetUserPreferenceToggle**(swUserPreferenceToggle\_e.swUseChangedDimensions,
True)
        swDrawing = swModel
        swDrawing.**IsolateChangedDimensions**()

        ' Save drawing document to another
name
        saveFileName =
"C:\Users\Public\Documents\SOLIDWORKS\SOLIDWORKS
2018\samples\tutorial\api\box\_changed.slddrw"
        swModelDocExt = swModel.**Extension**
        status = swModelDocExt.**SaveAs**(saveFileName,
swSaveAsVersion\_e.swSaveAsCurrentVersion,
swSaveAsOptions\_e.swSaveAsOptions\_Silent,
Nothing, errors, warnings)
        swApp.**CloseDoc**(saveFileName)

        ' Open the part document referenced
by the drawing document,
        '
change a dimension, and save the document
        fileName =
"C:\Users\Public\Documents\SOLIDWORKS\SOLIDWORKS
2018\samples\tutorial\api\box.sldprt"
        swModel = swApp.**OpenDoc6**(fileName,
swDocumentTypes\_e.swDocPART, swOpenDocOptions\_e.swOpenDocOptions\_Silent,
"",
errors, warnings)
        swModelDocExt = swModel.**Extension**
        status = swModelDocExt.**SelectByID2**("Sketch1",
"SKETCH",
0, 0, 0, True,
0, Nothing,
0)
        status = swModelDocExt.**SelectByID2**("D2@Sketch1@box.SLDPRT",
"DIMENSION",
-0.03613329319351, -0.02215939491444, 0.02938582119709,
True, 0,
Nothing, 0)
        Dim
swDimension As
Dimension
        swDimension = swModel.**Parameter**("D2@Sketch1")
        swDimension.**SystemValue** = 0.185
        swModel.ClearSelection2(True)
        status = swModel.**EditRebuild3**()
        status = swModel.**Save3**(swSaveAsOptions\_e.swSaveAsOptions\_Silent,
errors, warnings)
        swApp.**CloseDoc**(fileName)

        ' Open the previously saved drawing
document
        '
and place your cursor on the changed dimension,
        '
which displays in the color specified for
        '
changed dimensions, to see its previous value
        swModel = swApp.**OpenDoc6**(saveFileName,
swDocumentTypes\_e.swDocDRAWING, swOpenDocOptions\_e.swOpenDocOptions\_Silent,
"",
errors, warnings)
    End
Sub

    '''
<summary>
    '''
The SldWorks swApp variable is pre-assigned for you.
    '''
</summary>
    Public
swApp As
SldWorks

End
Class