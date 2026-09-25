<!-- source: sldworksapi/Add_Autoballoon_to_Face_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Add Auto Balloons to Drawing Example (VB.NET)

This example shows how to automatically add BOM balloons to a drawing view.

'------------------------------------------------------------------------------
' Preconditions: Open a drawing with a bill of materials (BOM) table.
'
' Postconditions: BOM balloons are added to the view.
'------------------------------------------------------------------------------
Imports
SolidWorks.Interop.sldworks
Imports
SolidWorks.Interop.swconst
Imports
System.Runtime.InteropServices
Imports
System

Partial
Class
SolidWorksMacro

    Dim
Part As
ModelDoc2
    Dim
vNotes As
Object
    Dim
autoballoonParams As
AutoBalloonOptions
    Dim
boolstatus As
Boolean

    Sub
main()

        Part = swApp.ActiveDoc
        boolstatus = Part.ActivateView("Drawing
View1")
        boolstatus = Part.Extension.SelectByID2("Drawing
View1",
"DRAWINGVIEW", 0, 0, 0,
False, 0,
Nothing, 0)

        autoballoonParams = Part.**CreateAutoBalloonOptions**()
        autoballoonParams.**Layout** =
swBalloonLayoutType\_e.swDetailingBalloonLayout\_Square
        autoballoonParams.**ReverseDirection** =
False
        autoballoonParams.**IgnoreMultiple**
= True
        autoballoonParams.**InsertMagneticLine**
= True
        autoballoonParams.**LeaderAttachmentToFaces**
= True
        autoballoonParams.**Style** =
swBalloonStyle\_e.swBS\_Circular
        autoballoonParams.**Size** = swBalloonFit\_e.swBF\_5Chars
        autoballoonParams.**UpperTextContent** =
swBalloonTextContent\_e.swBalloonTextItemNumber
        autoballoonParams.**Layername**
= "-None-"
        autoballoonParams.**ItemNumberStart**
= 1
        autoballoonParams.**ItemNumberIncrement** = 1
        autoballoonParams.**ItemOrder** =
swBalloonItemNumbersOrder\_e.swBalloonItemNumbers\_DoNotChangeItemNumbers
        autoballoonParams.**EditBalloons**
= True
        autoballoonParams.**EditBalloonOption**
= swEditBalloonOption\_Resequence

        vNotes = Part.**AutoBalloon5**(autoballoonParams)

    End
Sub

    Public
swApp As
SldWorks

End
Class