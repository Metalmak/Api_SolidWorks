<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSaveAsOptions.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IAdvancedSaveAsOptions Interface | |
| [See Also](#seealsobookmark)  [Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSaveAsOptions_members.html) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IAdvancedSaveAsOptions Interface |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Allows access to all **File > Save As** options when saving a SOLIDWORKS Part, Assembly, or Drawing.

**NOTE:** Click the **Members** link, located near the top of the topic, to see this interface's methods and properties.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Interface IAdvancedSaveAsOptions ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IAdvancedSaveAsOptions ``` | |

| C# |  |
| --- | --- |
| ``` public interface IAdvancedSaveAsOptions ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public interface class IAdvancedSaveAsOptions ``` | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See AdvancedSaveAsOptions.

# ![](dotnetimages/collapse.gif)Example

'VBA

'This example shows how to save a drawing with advanced options.
'--------------------------------------------------------------
' Preconditions:
' 1. Open:
'    *public\_documents***\samples\tutorial\advdrawings\foodprocessor.slddrw**
' 2. Open the Immediate window.
'
' Postconditions:
' 1. Inspect the Immediate window for the list of reference components,
'    before and after name modifications to the drawing and its template.
' 2. Inspect the DrwSavedFolder and Ref sub-folders. In those
'     directories, the names of top-level documents are changed to "SamplePart.\*".
'     The reference component names are changed to include a "Prff\_" prefix and
'     a "\_Suff" suffix.
'
' NOTE: Because the drawing and template are used elsewhere,
' do not save changes.
'--------------------------------------------------------------

Dim swApp As SldWorks.SldWorks
Dim swModel As ModelDoc2
Dim ModelExt As ModelDocExtension

Dim AdvOptData As AdvancedSaveAsOptions
Dim aFileName As String
Dim OrFileName As String
Dim Opt As Long
Dim Error As Long
Dim Warning As Long
Dim Status As Boolean
Dim i As Long
Dim k As Long

Const Suff As String = "\_Suff"
Const Prff As String = "Prff\_"
Option Explicit

Sub main()

    Dim DrwExtArr As Variant
    DrwExtArr = Array(".slddrw", ".drwdot")

    Set swApp = Application.SldWorks
    Set swModel = swApp.ActiveDoc
    Set ModelExt = swModel.Extension

    OrFileName = Left(swModel.GetPathName(), InStrRev(swModel.GetPathName(), "\"))
    Debug.Print OrFileName

    Dim IDList As Variant
    Dim fileNameList As Variant
    Dim pathNameList As Variant

     If Dir(OrFileName & "DrwSavedFolder", vbDirectory) = "" Then
            MkDir (OrFileName & "DrwSavedFolder")
            MkDir (OrFileName & "Ref")
        End If

    For i = 0 To UBound(DrwExtArr)

        aFileName = OrFileName & "DrwSavedFolder\SamplePart" & DrwExtArr(i)
        Debug.Print aFileName

        Set AdvOptData = ModelExt.**GetAdvancedSaveAsOptions**((1 + 2 + 4))

        AdvOptData.**SaveAllAsCopy** = True

        AdvOptData.**GetItemsNameAndPath** IDList, fileNameList, pathNameList

        PrintList fileNameList, pathNameList

        AdvOptData.**SetPrefixSuffixToAll** Prff, Suff

        AdvOptData.**GetItemsNameAndPath** IDList, fileNameList, pathNameList

        For k = 0 To UBound(IDList)

            If k = 0 Then ' For setting root folder and root file name
                pathNameList(k) = OrFileName & "DrwSavedFolder"
                fileNameList(k) = "SamplePart" & DrwExtArr(i)
            Else
                pathNameList(k) = OrFileName & "Ref"
            End If

        Next

        Error = AdvOptData.**ModifyItemsNameAndPath**(IDList, fileNameList, pathNameList)

        Debug.Print "Modify Paths Status : " & Error
        Debug.Print " "
        AdvOptData.**GetItemsNameAndPath** IDList, fileNameList, pathNameList

        PrintList fileNameList, pathNameList

        SaveFunctionCall (DrwExtArr(i))

        Debug.Print " "

    Next

    Debug.Print "Total Count " & i

End Sub

Sub SaveFunctionCall(Typ As String)

    Opt = (1 + 2)
    Debug.Print aFileName
    Status = ModelExt.**SaveAs3**(aFileName, 0, Opt, Nothing, AdvOptData, Error, Warning)

    Debug.Print "Save Status for Type " & Typ & " is : " & Status & " " & Error & " " & Warning

End Sub

Sub PrintList(sList As Variant, sList2 As Variant)

    Dim j As Long

    For j = 0 To UBound(sList)

        Debug.Print sList(j) & " \*\*>>\*\* " & sList2(j)

    Next

    Debug.Print "Total Count in the List is : " & j

End Sub

# ![](dotnetimages/collapse.gif)Accessors

[IModelDocExtension::GetAdvancedSaveAsOptions](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetAdvancedSaveAsOptions.html)

# ![](dotnetimages/collapse.gif)Access Diagram

[AdvancedSaveAsOptions](SWObjectModel.pdf#AdvancedSaveAsOptions)

# ![](dotnetimages/collapse.gif)See Also

####

[IAdvancedSaveAsOptions Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IAdvancedSaveAsOptions_members.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)