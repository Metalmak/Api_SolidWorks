<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2~DisableHighlight.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DisableHighlight Property (IBody2) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html) : DisableHighlight Property (IBody2) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Disables highlighting of the selected body in the graphics area.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property DisableHighlight As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IBody2 Dim value As System.Boolean   instance.DisableHighlight = value   value = instance.DisableHighlight ``` | |

| C# |  |
| --- | --- |
| ``` System.bool DisableHighlight {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool DisableHighlight {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to disable highlighting, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

**Visual Basic for Applications (VBA)**

'--------------------------------------------

'

' Preconditions: Model document is open and

'                contains at least one body.

'

' Postconditions: None

'

'--------------------------------------------

Option Explicit

Dim swApp As SldWorks.SldWorks
Dim swPart As SldWorks.PartDoc
Dim swBody As SldWorks.Body2
Dim swModel As SldWorks.ModelDoc2
Dim swModelDocExt As SldWorks.ModelDocExtension
Dim vBodies As Variant
Dim i As Long
Dim sBodySelStr As String, sBodyTypeSelStr As String
Dim bRet As Boolean

Sub main()

Set swApp = Application.SldWorks
Set swPart = swApp.**ActiveDoc**
Set swModel = swPart

vBodies = swPart.**GetBodies2**(swAllBodies, True)
If IsEmpty(vBodies) Then End

Set swModelDocExt = swModel.Extension

For i = 0 To UBound(vBodies)
        Set swBody = vBodies(i)
        sBodySelStr = swBody.**GetSelectionId**
        Select Case swBody.**GetType**
            Case swSolidBody
                sBodyTypeSelStr = "SOLIDBODY"
            Case swSheetBody
                sBodyTypeSelStr = "SURFACEBODY"
            Case Else
                Debug.Assert False
        End Select

        ' Select a body
        bRet = swModelDocExt.**SelectByID2**(sBodySelStr, sBodyTypeSelStr, 0#, 0#, 0#, True, 0, Nothing, swSelectOptionDefault): Debug.Assert bRet
        ' Disable highlighting of the body
        swBody.**DisableHighlight** = True

        ' Select the body again to check that highlighting is off
        swModel.**ClearSelection2** True
        bRet = swModelDocExt.**SelectByID2**(sBodySelStr, sBodyTypeSelStr, 0#, 0#, 0#, True, 0, Nothing, swSelectOptionDefault): Debug.Assert bRet

        ' Re-enable highlighting of the body
        swBody.**DisableHighlight** = False

        ' Select the body again to check that highlighting is on
        swModel.**ClearSelection2** True
        bRet = swModelDocExt.**SelectByID2**(sBodySelStr, sBodyTypeSelStr, 0#, 0#, 0#, True, 0, Nothing, swSelectOptionDefault): Debug.Assert bRet

       swModel.**ClearSelection2** True

    Next i

End Sub

# ![](dotnetimages/collapse.gif)See Also

####

[IBody2 Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2.html)

[IBody2 Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IBody2_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2009 FCS, Revision Number 17.0