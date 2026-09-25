<!-- source: sldworksapi/Create_PropertyManager_Page_Example_VB.htm -->

# SOLIDWORKS API Help

# Create PropertyManager Page Example (VBA)

This example shows how to create a PropertyManager
page that contains these controls:

* ActiveX
* Bitmap
* Bitmap buttons
* Button
* Combo box
* Group box
* Label
* List box
* Number box
* Radio button
* Selection box
* Slider
* Tab

This
example also shows how to handle focus events for these controls.

NOTE: If the model is an assembly
that contains multiple components, and you want to allow the user to
select edges, faces, or vertices, then you must specify swSelectType\_e.swSelCOMPSDONTOVERRIDE
for parameter SelType of IPropertyManagerPageSelectionbox::SetSelectionFilters.
Otherwise, if the user attempts to select an edge, face, or vertex, then the
entire component might get selected and not the edge, face, or vertex. This
example demonstrates how to specify SelType.

'--------------------------------------------------------------------------
' Preconditions:
'  1.
Copy and paste [Main](#Modules) into your project.
'  2. Insert a class and copy and paste
[Class1](#ClassModules) into that
class.
'  3. Click
Tools > References, select

'     SOLIDWORKS
version exposed
type libraries for add-in use, and click **OK**.
'  4. Verify that the specified assembly document exists.
'  5. Open an Immediate window.
'
' Postconditions:
'  1. Opens the
specified assembly.
'  2. Creates a PropertyManager page.
'  3. Creates the specified controls.
'  4. Examine the Immediate Window as you
use the specified controls.
'     Note the size of the button at the bottom of the
PropertyManager page.
'  5. Click **OK** to close the PropertyManager page.
'  6. Exit SOLIDWORKS.
'
' NOTE: Because the assembly document is used elsewhere,
' do not save changes
'----------------------------------------------------------------------------

'Main
Option Explicit

```
Public swApp As SldWorks.SldWorks
Public Part As SldWorks.ModelDoc2
Public pm As Class1
```

```
Sub main()
```

```
    Dim openDocErrors As Long
    Dim OpenDocWarnings As Long
```

```
    Set swApp = Application.SldWorks
    Set Part = swApp.OpenDoc6("C:\Users\Public\Documents\SOLIDWORKS\SOLIDWORKS 2018\samples\tutorial\advdrawings\bladed shaft.sldasm", swDocASSEMBLY, swOpenDocOptions_Silent, "", openDocErrors, OpenDocWarnings)
```

```
    'Create a new instance of the PropertyManager class
    Set pm = New Class1
    pm.Show
```

```
End Sub
```

[Back to top](#Top)

'Class1

Option Explicit

' Handler for PropertyManager page controls
Implements PropertyManagerPage2Handler9

' Control objects required for the PropertyManager page
Dim pm\_Page As PropertyManagerPage2
Dim pm\_Group As PropertyManagerPageGroup
Dim pm\_Selection As PropertyManagerPageSelectionbox
Dim pm\_Selection2 As PropertyManagerPageSelectionbox
Dim pm\_Label As PropertyManagerPageLabel
Dim pm\_Combo As PropertyManagerPageCombobox
Dim pm\_List As PropertyManagerPageListbox
Dim pm\_Number As PropertyManagerPageNumberbox
Dim pm\_Radio As PropertyManagerPageOption
Dim pm\_Slider As PropertyManagerPageSlider
Dim pm\_Tab As PropertyManagerPageTab
Dim pm\_Button As PropertyManagerPageButton
Dim pm\_BMPButton As PropertyManagerPageBitmapButton
Dim pm\_BMPButton2 As PropertyManagerPageBitmapButton
Dim pm\_Bitmap As PropertyManagerPageBitmap
Dim pm\_ActiveX As PropertyManagerPageActiveX
Dim ClickedCancel As Boolean
Dim retVal As Long

' Each control in the page needs a unique ID
Const GroupID As Long = 1
Const LabelID As Long = 2
Const SelectionID As Long = 3
Const ComboID As Long = 4
Const ListID As Long = 5
Const Selection2ID As Long = 6
Const NumberID As Long = 7
Const RadioID As Long = 8
Const SliderID As Long = 9
Const TabID As Long = 10
Const ButtonID As Long = 11
Const BMPButtonID As Long = 12
Const BMPButtonID2 As Long = 13
Const BitmapID As Long = 14
Const ActiveXID As Long = 15

Sub Show()

    pm\_Page.**Show2** 0

End Sub

' Run when a new instance of the class is
created

Private Sub Class\_Initialize()

    Dim PageTitle As String
    Dim caption As String
    Dim tip As String
    Dim options As Long
    Dim longerrors As Long
    Dim controlType As Long
    Dim alignment As Long
    Dim listItems(3) As String

    ' Set the variables for the page
    PageTitle = "Comps"

    options = swPropertyManager\_OkayButton \_
        + swPropertyManager\_CancelButton \_
        + swPropertyManagerOptions\_LockedPage
\_
        +
swPropertyManagerOptions\_PushpinButton

    ' Create the PropertyManager page
    Set pm\_Page = swApp.**CreatePropertyManagerPage**(PageTitle,
\_
        options, Me, longerrors)

    ' Make sure that the page was created properly
    If longerrors = swPropertyManagerPage\_Okay Then

        ' Add controls to
the page

        ' Add a tab
        Set pm\_Tab =
pm\_Page.**AddTab**(TabID, "Application", "", 0)

        ' Add a group box to the tab
        caption =
"Controls"
        options =
swGroupBoxOptions\_Visible + \_

swGroupBoxOptions\_Expanded
        Set pm\_Group =
pm\_Tab.**AddGroupBox**(GroupID, caption, options)

        ' Add two selection boxes
        controlType =
swControlType\_Selectionbox
        caption = ""

        alignment =
swControlAlign\_Indent
        options =
swControlOptions\_Visible + \_

swControlOptions\_Enabled
        tip = "Select an
edge, face, vertex, solid body, or a component"
        Set pm\_Selection =
pm\_Group.**AddControl2**(SelectionID, \_

controlType, caption, alignment, options, tip)

        Set pm\_Selection2
= pm\_Group.**AddControl2**(Selection2ID, \_

controlType, caption, alignment, options, tip)

        Dim filters(6) As
Long
        filters(0) = swSelEDGES
        filters(1) = swSelREFEDGES
        filters(2) = swSelFACES
        filters(3) = swSelVERTICES
        filters(4) = swSelSOLIDBODIES
        filters(5) = swSelCOMPONENTS
        filters(6) = swSelCOMPSDONTOVERRIDE

        pm\_Selection.**SingleEntityOnly**
= False
        pm\_Selection.**AllowMultipleSelectOfSameEntity**
= True
        pm\_Selection.**Height** = 50
        pm\_Selection.**SetSelectionFilters**
filters
        pm\_Selection2.**SingleEntityOnly**
= False
        pm\_Selection2.**AllowMultipleSelectOfSameEntity**
= True
        pm\_Selection2.**Height** = 50
        pm\_Selection2.**SetSelectionFilters**
filters

        ' Add a combo box
        controlType =
swControlType\_Combobox
        caption = ""
        alignment =
swControlAlign\_Indent
        options =
swControlOptions\_Visible + \_

swControlOptions\_Enabled
        tip = "Select a
value"

        Set pm\_Combo =
pm\_Group.**AddControl2**(ComboID, \_

controlType, caption, alignment, options, tip)

        If Not pm\_Combo Is
Nothing Then

pm\_Combo.**Height** = 50

listItems(0) = "Value 1"
            listItems(1)
= "Value 2"
            listItems(2)
= "Value 3"
            listItems(3)
= "Value 4"

pm\_Combo.**AddItems** (listItems)
            pm\_Combo.**CurrentSelection**
= 0

        End If

        ' Add a list box
        controlType =
swControlType\_Listbox
        caption = ""
        alignment =
swControlAlign\_Indent
        options =
swControlOptions\_Visible + \_

swControlOptions\_Enabled
        tip =
"Multi-select values in the list box"

        Set pm\_List =
pm\_Group.**AddControl2**(ListID, \_

controlType, caption, alignment, options, tip)
        pm\_List.**Style** =
swPropMgrPageListBoxStyle\_MultipleItemSelect
        pm\_List.**Height** = 50

        If Not pm\_List Is Nothing Then

pm\_List.**Height** = 50
            listItems(0)
= "Value 1"
            listItems(1)
= "Value 2"
            listItems(2)
= "Value 3"
            listItems(3)
= "Value 4"
            pm\_List.**AddItems**
(listItems)
            pm\_List.**SetSelectedItem**
1, True

        End If

        ' Add a label
        Set pm\_Label = pm\_Group.**AddControl2**(LabelID,
swControlType\_Label, "Label", swControlAlign\_LeftEdge, options, "")

        ' Add a slider
        Set pm\_Slider = pm\_Group.**AddControl2**(SliderID,
swControlType\_Slider, "Slider", swControlAlign\_LeftEdge, options, "Slide")

        ' Add a radio
button
        Set pm\_Radio = pm\_Group.**AddControl2**(RadioID,
swControlType\_Option, "Radio button", swControlAlign\_LeftEdge, options,
"Select")

        ' Add a number box
        Set pm\_Number = pm\_Group.**AddControl2**(NumberID,
swControlType\_Numberbox, "Number box", swControlAlign\_LeftEdge, options, "Spin")

        ' Add a button
        Set pm\_Button = pm\_Group.**AddControl2**(ButtonID,
swControlType\_Button, "Button", swControlAlign\_LeftEdge, options, "Click")

        ' Add a bitmap
button
        Set pm\_BMPButton = pm\_Group.**AddControl2**(BMPButtonID,
swControlType\_BitmapButton, "Bitmap button", swControlAlign\_LeftEdge, options,
"Click")
        pm\_BMPButton.**SetStandardBitmaps**
(swPropertyManagerPageBitmapButtons\_e.swBitmapButtonImage\_parallel)

        ' Add a bitmap
        Set pm\_Bitmap = pm\_Group.**AddControl2**(BitmapID,
swControlType\_Bitmap, "Bitmap", swControlAlign\_LeftEdge, options, "Bitmap")
        pm\_Bitmap.**SetStandardBitmap** (swBitmapControlStandardTypes\_e.swBitmapControl\_Volume)

        ' To add an ActiveX
control, uncomment the following two lines and modify *ClassID* and *LicenseKey* parameters
for your ActiveX control.
       ' Set pm\_ActiveX = pm\_Group.**AddControl2**(ActiveXID,
swControlType\_ActiveX, "ActiveX", swControlAlign\_LeftEdge, options, "ActiveX
control tip")
       ' pm\_ActiveX.**SetClass** "*ClassID*",
"*LicenseKey*"

       ' To add another bitmap button that scales with your computer's resolution,
uncomment the 10 code lines below and replace the

' ImageList and ImageListMasks array elements with the pathnames of scaled image
files. After running this macro, change the

' screen resolution of your computer. Log off and back in. Start SOLIDWORKS and
run this macro again. Notice how this button

' control scales with screen resolution.

' Set pm\_BMPButton2 = pm\_Group.**AddControl2**(BMPButtonID2, swControlType\_BitmapButton, "Bitmap button", swControlAlign\_LeftEdge, options, "Click")

' Dim imageList(2) As String
       ' Dim imageListMasks(2) As String

' imageList(0) = "*Pathname\_to\_nxn\_image*"

' imageList(1) = "*Pathname\_to\_nnxnn\_image*"

' imageList(2) = "*Pathname\_to\_nnnxnnn\_image*"

' imageListMasks(0) = "*Pathname\_to\_mask\_nxn\_image*"

' imageListMasks(1) = "*Pathname\_to\_mask\_nnxnn\_image*"

' imageListMasks(2) = "*Pathname\_to\_mask\_nnnxnnn\_image*"

' pm\_BMPButton2.**SetBitmapsByName3** imageList, imageListMasks

    Else

        MsgBox "An error
occurred while attempting to create the PropertyManager Page", vbCritical

    End If

End Sub

Private Sub PropertyManagerPage2Handler9\_**AfterActivation**()

End Sub

Private Sub PropertyManagerPage2Handler9\_**AfterClose**()

    ' Destroy the class
    Set pm = Nothing

End Sub

Private Function PropertyManagerPage2Handler9\_**OnActiveXControlCreated**(ByVal
Id As Long, ByVal Status As Boolean) As Long
    Debug.Print "ActiveX control created"
End Function

Private Sub PropertyManagerPage2Handler9\_**OnButtonPress**(ByVal
Id As Long)
    Debug.Print "Button clicked"
End Sub

Private Sub PropertyManagerPage2Handler9\_**OnCheckboxCheck**(ByVal
Id As Long, ByVal Checked As Boolean)

End Sub

Private Sub PropertyManagerPage2Handler9\_**OnClose**(ByVal
Reason As Long)

    If Reason =
swPropertyManagerPageClose\_Cancel Then

        ' Cancel button
clicked
        ClickedCancel = True

    ElseIf Reason =
swPropertyManagerPageClose\_Okay Then

        ' OK button
clicked
        ClickedCancel = False

    End If

End Sub

Private Sub PropertyManagerPage2Handler9\_**OnComboboxEditChanged**(ByVal
Id As Long, ByVal Text As String)

End Sub

Private Sub PropertyManagerPage2Handler9\_**OnComboboxSelectionChanged**(ByVal
Id As Long, ByVal Item As Long)

End Sub

Private Sub PropertyManagerPage2Handler9\_**OnGroupCheck**(ByVal
Id As Long, ByVal Checked As Boolean)

End Sub

Private Sub PropertyManagerPage2Handler9\_**OnGroupExpand**(ByVal
Id As Long, ByVal Expanded As Boolean)

End Sub

Private Function PropertyManagerPage2Handler9\_**OnHelp**() As Boolean

End Function

Private Function PropertyManagerPage2Handler9\_**OnKeystroke**(ByVal
Wparam As Long, ByVal Message As Long, ByVal Lparam As Long, ByVal Id As Long)
As Boolean

End Function

Private Sub PropertyManagerPage2Handler9\_**OnListboxSelectionChanged**(ByVal
Id As Long, ByVal Item As Long)

End Sub

Private Function PropertyManagerPage2Handler9\_**OnNextPage**()
As Boolean

End Function

Private Sub PropertyManagerPage2Handler9\_**OnNumberboxChanged**(ByVal
Id As Long, ByVal Value As Double)
    Debug.Print "Number box changed"
End Sub

Private Sub PropertyManagerPage2Handler9\_**OnOptionCheck**(ByVal
Id As Long)
    Debug.Print "Option selected"
End Sub

Private Sub PropertyManagerPage2Handler9\_**OnPopupMenuItem**(ByVal
Id As Long)

End Sub

Private Sub PropertyManagerPage2Handler9\_**OnPopupMenuItemUpdate**(ByVal
Id As Long, retVal As Long)

End Sub

Private Function PropertyManagerPage2Handler9\_**OnPreview**()
As Boolean

End Function

Private Function PropertyManagerPage2Handler9\_**OnPreviousPage**()
As Boolean

End Function

Private Sub PropertyManagerPage2Handler9\_**OnRedo**()

End Sub

Private Sub PropertyManagerPage2Handler9\_**OnSelectionboxCalloutCreated**(ByVal
Id As Long)

End Sub

Private Sub PropertyManagerPage2Handler9\_**OnSelectionboxCalloutDestroyed**(ByVal
Id As Long)

End Sub

Private Sub PropertyManagerPage2Handler9\_**OnSelectionboxFocusChanged**(ByVal
Id As Long)

    Debug.Print "The focus moved to selection
box " & Id

End Sub

Private Sub PropertyManagerPage2Handler9\_**OnSelectionboxListChanged**(ByVal
Id As Long, ByVal Count As Long)
    pm\_Page.**SetCursor** (swPropertyManagerPageCursors\_Advance)

    Debug.Print "The list in selection box " &
Id & " changed"

End Sub

Private Sub PropertyManagerPage2Handler9\_**OnSliderPositionChanged**(ByVal
Id As Long, ByVal Value As Double)
    Debug.Print "Slider position changed"
End Sub

Private Sub PropertyManagerPage2Handler9\_**OnSliderTrackingCompleted**(ByVal
Id As Long, ByVal Value As Double)

End Sub

Private Function PropertyManagerPage2Handler9\_**OnSubmitSelection**(ByVal
Id As Long, ByVal Selection As Object, ByVal SelType As Long, ItemText As
String) As Boolean

    PropertyManagerPage2Handler9\_**OnSubmitSelection**
= True

End Function

Private Function PropertyManagerPage2Handler9\_**OnTabClicked**(ByVal
Id As Long) As Boolean

End Function

Private Sub PropertyManagerPage2Handler9\_**OnTextboxChanged**(ByVal
Id As Long, ByVal Text As String)

End Sub

Private Sub PropertyManagerPage2Handler9\_**OnUndo**()

End Sub

Private Sub PropertyManagerPage2Handler9\_**OnWhatsNew**()

End Sub

Private Sub PropertyManagerPage2Handler9\_**OnLostFocus**(ByVal
Id As Long)

    Debug.Print "Control box " & Id & " lost
focus"

End Sub

Private Sub PropertyManagerPage2Handler9\_**OnGainedFocus**(ByVal
Id As Long)

   Dim varArray As Variant

   Debug.Print "Control box " & Id & " gained
focus"

   varArray = pm\_List.**GetSelectedItems**

   pm\_Combo.**CurrentSelection** = varArray(0)

End Sub

Public Sub PropertyManagerPage2Handler9\_**OnListBoxRMBUp**(ByVal
Id As Long, ByVal posX As Long, ByVal posY As Long)

End Sub

Public Function PropertyManagerPage2Handler9\_**OnWindowFromHandleControlCreated**(ByVal
Id As Long, ByVal Status As Boolean) As Long

End Function

Public Sub PropertyManagerPage2Handler9\_O**nNumberboxTrackingCompleted**(ByVal
Id As Long, ByVal Value As Double)

End Sub

[Back to top](#Top)