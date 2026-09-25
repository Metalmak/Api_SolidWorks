<!-- source: sldworksapi/Attach_Annotation_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Attach Annotation Example (VB.NET)

This example shows how to attach an existing annotation to a drawing view.

'----------------------------------------------------------------------------
' Preconditions: Open *public\_documents***\samples\tutorial\api\replaceview.slddrw**.
'
' Postconditions:
' 1. Inserts a note annotation in the drawing.
' 2. Selects the annotation.
' 3. Appends a face in a drawing view to the selection list.
' 4. Attaches the annotation to the selected face.
' 5. Examine the drawing.
' 6. Close the drawing without saving it.
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

Partial
Class
SolidWorksMacro

    Dim
part As
ModelDoc2
    Dim
draw As
DrawingDoc
    Dim
aNote As
Note
    Dim
anAnnot As
Annotation
    Dim
selectData As
SelectData
    Dim ret
As
Integer
    Dim
boolstatus As
Boolean

    Sub
main()

        part = swApp.**ActiveDoc**
        draw = part

        boolstatus = part.**ActivateSheet**("Sheet1")

        aNote = draw.**CreateText2**("This
is a note.", 0.21, 0.12, 0, 0.005, 0)
        anAnnot = aNote.**GetAnnotation**
        ret = anAnnot.**SetLeader3**(swLeaderStyle\_e.swBENT, swLeaderSide\_e.swLS\_SMART,
True,
False,
False,
False)

        anAnnot.**Select3**(False,
selectData)
        boolstatus = part.**ActivateView**("Drawing
View1")
        boolstatus = part.**Extension**.**SelectByID2**("",
"FACE",
0.0783563575357558, 0.17448024010205, -499.965138294658,
True, 0,
Nothing, 0)

        draw.**AttachAnnotation**(swAttachAnnotationOption\_e.swAttachAnnotationOption\_View)

    End
Sub

    Public
swApp As
SldWorks

End
Class