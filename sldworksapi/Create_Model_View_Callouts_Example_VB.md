<!-- source: sldworksapi/Create_Model_View_Callouts_Example_VB.htm -->

# SOLIDWORKS API Help

# Create a Callout in a Model View Example (VBA)

This example shows how to create a callout in a model view.

```
'----------------------------------------------------------------------------
' Preconditions:
' 1. Open a part document.
' 2. Select:
'    Tools > References > SOLIDWORKS <version> exposed type
'    libraries for add-in use.
' 3. Copy Class1 to a class module named CalloutHandler.
'
' Postconditions:
' 1. A callout with one row is created in the first model view.
' 2. Press F5 three more times to add a callout to three other model views.
'
' NOTE: Because the model is used elsewhere,
' do not save changes when closing it.
' ---------------------------------------------------------------------------
```

Option Explicit
Dim swApp As SldWorks.SldWorks
Dim swModelDoc As SldWorks.ModelDoc2
Dim swModelDocExtn As SldWorks.ModelDocExtension
Dim ViewMgr As ModelViewManager
Dim swModelView As ModelView
Dim Viewcallout As SldWorks.Callout
Dim handle As New CalloutHandler

Sub main()

    Set swApp = Application.SldWorks
    Set swModelDoc = swApp.ActiveDoc
    Set swModelDocExtn = swModelDoc.Extension

    Set ViewMgr = swModelDoc.ModelViewManager
    ViewMgr.ViewportDisplay =
swViewportDisplay\_e.swViewportFourView
    swModelDoc.GetModelViewCount
    Set swModelView = swModelDoc.GetFirstModelView
    While (Not swModelView Is Nothing)
        Set Viewcallout = swModelView.**CreateCallout**(1,
handle)
        Viewcallout.Label2(0) = "TEST"
        Viewcallout.SkipColon = False
        Viewcallout.ValueInactive(0) = True
        Call Viewcallout.SetTargetPoint(0,
0#, 0#, 0#)
        Viewcallout.Display (True)
        Stop
        Set swModelView = swModelView.GetNext
    Wend

End Sub

'Class1:

Implements SwCalloutHandler

Private Function SwCalloutHandler\_OnStringValueChanged(ByVal
pManipulator As Object, ByVal RowID As Long, ByVal Text As String) As Boolean

    Debug.Print ("Text: " & Text)
    Debug.Print ("Row: " & RowID)
    SwCalloutHandler\_OnStringValueChanged = True

End Function