<!-- source: sldworksapi/Insert_Weld_Symbol_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Insert Weld Symbol Example (VB.NET)

This example shows how to insert a weld symbol into a model.

'----------------------------------------------------------------------------
' Preconditions:
' 1. Open *public\_documents***\samples\tutorial\api\weldment\_box3.sldprt**.

' 2. Select a face, edge, or sketch segment for Weld Symbol insertion.
' 3. Open an Immediate window.
'
' Postconditions:
' 1. Inserts the specified ISO Weld Symbol.
' 2. Inspect the Immediate window.
'

' NOTE: Because the model is used elsewhere, do not save changes.

' ---------------------------------------------------------------------------
Imports SolidWorks.Interop.sldworks
Imports SolidWorks.Interop.swconst
Imports System.Runtime.InteropServices
Imports System
Imports System.Diagnostics

Partial Class SolidWorksMacro

    Sub main()

        Dim swModel As ModelDoc2
        Dim swWeldSymbol As WeldSymbol

        swModel = swApp.**ActiveDoc**
        swWeldSymbol = swModel.**InsertWeldSymbol3**

        swWeldSymbol.**SetFieldWeld**(swWeldSymbolField\_e.swFieldWeldNone)
        swWeldSymbol.**SetPeripheral**(False)
        swWeldSymbol.**SetProcess**(True, "Process", True)
        swWeldSymbol.**SetStagger**(True)
        swWeldSymbol.**SetSymmetric**(swWeldSymbolSymmetric\_e.swWeldSymmetric)
        swWeldSymbol.**SetText**(True, "Left", "BUTT", "Right", "Stagger", swWeldSymbolContourTypes\_e.swWeldContourNone)

        Debug.Print("Arc count: " & swWeldSymbol.**GetArcCount**)
        Debug.Print("Arrow head count: " & swWeldSymbol.**GetArrowHeadCount**)
        Debug.Print("Contour setting as defined in swWeldSymbolContourTypes\_e: " & swWeldSymbol.**GetContour**(True))
        Debug.Print("Field weld setting as defined in swWeldSymbolField\_e: " & swWeldSymbol.**GetFieldWeld**)
        Debug.Print("Number of leaders on this weld symbol: " & swWeldSymbol.**GetLeaderCount**)
        Debug.Print("Number of line segments in this weld symbol: " & swWeldSymbol.**GetLineCount**)
        Debug.Print("Weld all around the contour? " & swWeldSymbol.**GetPeripheral**)
        Debug.Print("Welding process indicated? " & swWeldSymbol.**GetProcess**)
        Debug.Print("Reference box around the specification process text? " & swWeldSymbol.**GetProcessReference**)
        Debug.Print("Stagger symbols above and below the line? " & swWeldSymbol.**GetStagger**)
        Debug.Print("Weld symbol symmetry as defined in swWeldSymbolSymmetric\_e: " & swWeldSymbol.**GetSymmetric**)
        Debug.Print("Number of text items in this weld symbol: " & swWeldSymbol.**GetTextCount**)
        Debug.Print("Number of triangles in this weld symbol: " & swWeldSymbol.**GetTriangleCount**)
        Debug.Print("Extra leader line? " & swWeldSymbol.**HasExtraLeader**)
        Debug.Print("Weld symbol is attached to a leaderline? " & swWeldSymbol.**IsAttached**)

    End Sub

    Public swApp As SldWorks

End Class