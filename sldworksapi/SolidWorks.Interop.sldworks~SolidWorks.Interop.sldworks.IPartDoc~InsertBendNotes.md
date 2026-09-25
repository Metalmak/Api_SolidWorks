<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc~InsertBendNotes.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| InsertBendNotes Method (IPartDoc) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html) : InsertBendNotes Method (IPartDoc) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FlatPatternFeature*
:   [IFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html)

Inserts bend notes for the specified flat-pattern feature of this sheet metal part.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function InsertBendNotes( _    ByVal FlatPatternFeature As System.Object _ ) As System.Object ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPartDoc Dim FlatPatternFeature As System.Object Dim value As System.Object   value = instance.InsertBendNotes(FlatPatternFeature) ``` | |

| C# |  |
| --- | --- |
| ``` System.object InsertBendNotes(     System.object FlatPatternFeature ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.Object^ InsertBendNotes(  &   System.Object^ FlatPatternFeature ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FlatPatternFeature*
:   [IFeature](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFeature.html)

#### Return Value

Array of [INote](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.INote.html)s

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PartDoc::InsertBendNotes.

# ![](dotnetimages/collapse.gif)Example

'VBA

' 1. Open a sheet metal part with a **Flat-Pattern1** feature.
' 2. Run the macro.
' 3. Inspect the Immediate window for the list of inserted bend notes.

Dim swApp As SldWorks.SldWorks
Dim Part As SldWorks.ModelDoc2
Dim myFlatPattern As SldWorks.Feature
Dim myBendNotes As Variant
Dim myAnno As SldWorks.Note
Dim boolstatus As Boolean
Dim i As Long
Option Explicit

Sub main()

    Set swApp = Application.SldWorks
    Set Part = swApp.ActiveDoc
    boolstatus = Part.Extension.SelectByID2("Flat-Pattern1", "BODYFEATURE", 0, 0, 0, False, 0, Nothing, 0)

    Set myFlatPattern = Part.SelectionManager.GetSelectedObject6(1, -1)
    If Not myFlatPattern Is Nothing Then
        myBendNotes = Part.**InsertBendNotes**(myFlatPattern)
        For i = 0 To UBound(myBendNotes)
            Set myAnno = myBendNotes(i)
            Debug.Print myAnno.GetName
        Next i
    End If

End Sub

# ![](dotnetimages/collapse.gif)See Also

####

[IPartDoc Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc.html)

[IPartDoc Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPartDoc_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2019 FCS, Revision Number 27.0