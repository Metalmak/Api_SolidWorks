<!-- source: sldworksapi/Get_Render_References_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Get Render References (VB.NET)

This example shows how to get the render stock (SOLIDWORKS-supplied)
references for a model.

'-------------------------------------------------
' Preconditions:
' 1. Verify that the specified part to open and
'    kitchen background scene files exist.
' 2. Open the Immediate window.
'
' Postconditions:
' 1. Inserts the kitchen background scene in the part.
' 2. Gets the names of the render references.
' 3. Examine the Immediate window.
'
' NOTE: Because the part is used elsewhere, do
' not save changes.
'--------------------------------------------------
Imports
SolidWorks.Interop.sldworks
Imports
SolidWorks.Interop.swconst
Imports System
Imports System.Diagnostics

Partial
Class SolidWorksMacro

    Public
Sub Main()

        Dim swModel
As ModelDoc2
        Dim swModelDocExt
As ModelDocExtension
        Dim modelName
As
String
        Dim
renderReferences As
Object
        Dim
status As
Boolean
        Dim
errors As
Long, warnings
As Long
        Dim
i As
Long

        modelName =
"C:\Users\Public\Documents\SOLIDWORKS\SOLIDWORKS 2018\samples\tutorial\api\toaster.sldprt"
        swModel = swApp.**OpenDoc6**(modelName,
swDocumentTypes\_e.swDocPART, swOpenDocOptions\_e.swOpenDocOptions\_Silent,
"", errors, warnings)
        swModelDocExt = swModel.**Extension**

        ' Insert kitchen background scene
        ' and rebuild the
model to see it
        status = swModelDocExt.**InsertScene**("C:\Program
Files\SOLIDWORKS Corp\SOLIDWORKS\data\graphics\scenes\03 presentation scenes\00
kitchen\_background.p2s")
        status = swModel.**ForceRebuild3**(True)

        ' Get the render
stock references for the
        ' kitchen
background scene and print
        ' them to the
Immediate window
        renderReferences = swModelDocExt.**GetRenderStockReferences**
        For i = 0
To UBound(renderReferences)
            Debug.Print("Render reference: "
& renderReferences(i))
        Next i

    End
Sub

    '''
<summary>
    ''' The SldWorks swApp
variable is pre-assigned for you.
    '''
</summary>
    Public
swApp As SldWorks

End
Class