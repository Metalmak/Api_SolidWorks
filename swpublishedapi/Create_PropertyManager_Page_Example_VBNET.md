<!-- source: swpublishedapi/Create_PropertyManager_Page_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Create PropertyManager Page Example (VB.NET)

This example shows how to create a PropertyManager
page that contains the following controls:

* ActiveX
* Bitmap
* Bitmap button
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
select edges, faces, or vertices, then you must specify swSelCOMPSDONTOVERRIDE
for parameter SelType of IPropertyManagerPageSelectionbox::SetSelectionFilters.
Otherwise, if the user attempts to select an edge, face, or vertex, then the
entire component might get selected and not the edge, face, or vertex. This
example demonstrates how to specify SelType.

'----------------------------------------------------------------------------
'
Preconditions:

' 1. Copy  [Modules - main](#Modules)
to your project.
' 2. Copy  [Class Modules
- clsPropMgr](#Class) to a class in your project.
' 3. Right-click the name of your project, select
'    Add Reference,
browse i*nstall\_dir***\api\redist\**, select

'    SolidWorks.Interop.swpublished.dll, and click
OK.
' 4. Ensure that the specified assembly document exists.
' 5. Modify *ClassID* and *LicenseKey*
parameters in
'    IPropertyManagerPageActiveX::SetClass to add your ActiveX
control
'    to the PropertyManager page.
' 6. Open an Immediate window.
'
'
Postconditions:

' 1. Creates a
PropertyManager page called **Comps**.
' 2. Creates the specified controls.
' 3. Inspect
the contents of **Comps** and the Immediate Window as
'    you
use the controls.
' 4. Click the green check mark to close the PropertyManager page.
'
' **NOTES:**
' \* After running
this macro, select
'   Tools > Options
> System Options > Stop VSTA debugger
'
  on
macro exit.
'
\* Because
the assembly document is used elsewhere,
'   do not save any
changes when closing the document.
'----------------------------------------------------------------------------

'Modules
- main

Imports SolidWorks.Interop.sldworks

Imports SolidWorks.Interop.swconst

Imports System

Partial Class SolidWorksMacro

    Public
Part As ModelDoc2

    Public
WithEvents pm As clsPropMgr

    Sub
main()

        Dim
openDocErrors As Integer

        Dim
OpenDocWarnings As Integer

        swApp.SetUserPreferenceToggle(swUserPreferenceToggle\_e.swStopDebuggingVstaOnExit,
False)

        Part
= swApp.OpenDoc6("C:\Users\Public\Documents\SOLIDWORKS\SOLIDWORKS
2018\samples\tutorial\advdrawings\bladed shaft.sldasm",
swDocumentTypes\_e.swDocASSEMBLY, swOpenDocOptions\_e.swOpenDocOptions\_Silent,
"", openDocErrors, OpenDocWarnings)

        'Create
a new instance of the PropertyManager class

        pm
= New clsPropMgr(swApp)

        pm.Show()

    End
Sub

    Public
swApp As SldWorks

End Class

[Back to top](#Top)

'Class
Modules - clsPropMgr

Imports SolidWorks.Interop.sldworks

Imports SolidWorks.Interop.swconst

Imports SolidWorks.Interop.swpublished

Imports System

Imports System.Runtime.InteropServices

Imports System.Diagnostics

<ComVisibleAttribute(True)> \_

Public Class clsPropMgr

    Implements
PropertyManagerPage2Handler9

    Dim
swApp As SldWorks

    'Control objects required for the PropertyManager page
    Dim pm\_Page As PropertyManagerPage2
    Dim pm\_Group As PropertyManagerPageGroup
    Dim pm\_Selection As PropertyManagerPageSelectionbox
    Dim pm\_Selection2 As PropertyManagerPageSelectionbox
    Dim pm\_Label As PropertyManagerPageLabel
    Dim pm\_Combo As PropertyManagerPageCombobox
    Dim pm\_List As PropertyManagerPageListbox
    Dim pm\_Number As PropertyManagerPageNumberbox
    Dim pm\_Radio As PropertyManagerPageOption
    Dim pm\_Slider As PropertyManagerPageSlider
    Dim pm\_Tab As PropertyManagerPageTab
    Dim pm\_Button As PropertyManagerPageButton
    Dim pm\_BMPButton As PropertyManagerPageBitmapButton
    Dim pm\_Bitmap As PropertyManagerPageBitmap
    Dim pm\_ActiveX As PropertyManagerPageActiveX

    'Each control in the page needs a unique ID
    Const GroupID As Integer = 1
    Const LabelID As Integer = 2
    Const SelectionID As Integer = 3
    Const ComboID As Integer = 4
    Const ListID As Integer = 5
    Const Selection2ID As Integer = 6
    Const NumberID As Integer = 7
    Const RadioID As Integer = 8
    Const SliderID As Integer = 9
    Const TabID As Integer = 10
    Const ButtonID As Integer = 11
    Const BMPButtonID As Integer = 12
    Const BitmapID As Integer = 13
    Const ActiveXID As Integer = 14

    Dim
ClickedCancel As Boolean

    Dim
retVal As Integer

    Sub
Show()

        pm\_Page.Show2(0)

    End
Sub

    'The
following runs when a new instance

    'of
the class is created

    Public
Sub New(ByVal swApp As SldWorks)

        Dim
PageTitle As String

        Dim
caption As String

        Dim
tip As String

        Dim
options As Integer

        Dim
longerrors As Integer

        Dim
controlType As Integer

        Dim
alignment As Integer

        Dim
listItems(3) As String

        'Set
the variables for the page

        PageTitle
= "Comps"

        options
= swPropertyManagerButtonTypes\_e.swPropertyManager\_OkayButton \_

            +
swPropertyManagerButtonTypes\_e.swPropertyManager\_CancelButton \_

            +
swPropertyManagerPageOptions\_e.swPropertyManagerOptions\_LockedPage \_

            +
swPropertyManagerPageOptions\_e.swPropertyManagerOptions\_PushpinButton

        'Create
the PropertyManager page

        pm\_Page
= CType(swApp.CreatePropertyManagerPage(PageTitle,
\_

            options,
Me, longerrors), PropertyManagerPage2)

        'Make
sure that the page was created properly

        If
longerrors = swPropertyManagerPageStatus\_e.swPropertyManagerPage\_Okay
Then

            'Add the controls to the page

'Add a tab
            pm\_Tab = pm\_Page.**AddTab**(TabID, "Application", "", 0)

            'Add a group box to the tab
            caption = "Controls"
            options = swAddGroupBoxOptions\_e.swGroupBoxOptions\_Visible + \_
                swAddGroupBoxOptions\_e.swGroupBoxOptions\_Expanded
            pm\_Group = pm\_Tab.**AddGroupBox**(GroupID, caption, options)

            'Add
two selection boxes

            controlType
= swPropertyManagerPageControlType\_e.swControlType\_Selectionbox

            caption
= ""  '
No caption for selection boxes

            alignment
= swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_Indent

            options
= swAddControlOptions\_e.swControlOptions\_Visible + \_

                swAddControlOptions\_e.swControlOptions\_Enabled

            tip
= "Select an edge, face, vertex, solid body, or a component"

            pm\_Selection
= pm\_Group.AddControl2(SelectionID,
\_

                controlType,
caption, alignment, options, tip)

            pm\_Selection2
= pm\_Group.AddControl2(Selection2ID,
\_

                controlType,
caption, alignment, options, tip)

            Dim
filters(6) As swSelectType\_e

            filters(0)
= swSelectType\_e.swSelEDGES

            filters(1)
= swSelectType\_e.swSelREFEDGES

            filters(2)
= swSelectType\_e.swSelFACES

            filters(3)
= swSelectType\_e.swSelVERTICES

            filters(4)
= swSelectType\_e.swSelSOLIDBODIES

            filters(5)
= swSelectType\_e.swSelCOMPONENTS

            filters(6)
= swSelectType\_e.swSelCOMPSDONTOVERRIDE

            Dim
filterObj As Object

            filterObj
= filters

            pm\_Selection.SingleEntityOnly = False

            pm\_Selection.AllowMultipleSelectOfSameEntity = True

            pm\_Selection.Height = 50

            pm\_Selection.SetSelectionFilters(filterObj)

            pm\_Selection2.SingleEntityOnly = False

            pm\_Selection2.AllowMultipleSelectOfSameEntity = True

            pm\_Selection2.Height = 50

            pm\_Selection2.SetSelectionFilters(filterObj)

            'Add a combo box

            controlType
= swPropertyManagerPageControlType\_e.swControlType\_Combobox

            caption
= ""

            alignment
= swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_Indent

            options
= swAddControlOptions\_e.swControlOptions\_Visible + \_

                swAddControlOptions\_e.swControlOptions\_Enabled

            tip
= "Select a value"

            pm\_Combo
= pm\_Group.AddControl2(ComboID,
\_

                controlType,
caption, alignment, options, tip)

            If
Not pm\_Combo Is Nothing Then

                pm\_Combo.Height = 50

                listItems(0)
= "Value 1"

                listItems(1)
= "Value 2"

                listItems(2)
= "Value 3"

                listItems(3)
= "Value 4"

                pm\_Combo.AddItems(listItems)

                pm\_Combo.CurrentSelection = 0

            End
If

            'Add a list box

            controlType
= swPropertyManagerPageControlType\_e.swControlType\_Listbox

            caption
= ""

            alignment
= swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_Indent

            options
= swAddControlOptions\_e.swControlOptions\_Visible + \_

                swAddControlOptions\_e.swControlOptions\_Enabled

            tip
= "Multi-select values in the list box"

            pm\_List
= pm\_Group.AddControl2(ListID,
\_

                controlType,
caption, alignment, options, tip)

            pm\_List.Style = swPropMgrPageListBoxStyle\_e.swPropMgrPageListBoxStyle\_MultipleItemSelect

            pm\_List.Height = 50

            If
Not pm\_List Is Nothing Then

                pm\_List.Height = 50

                listItems(0)
= "Value 1"

                listItems(1)
= "Value 2"

                listItems(2)
= "Value 3"

                listItems(3)
= "Value 4"

                pm\_List.AddItems(listItems)

                pm\_List.SetSelectedItem(1, True)

            End
If

'Add a label
            pm\_Label = pm\_Group.**AddControl2**(LabelID, swPropertyManagerPageControlType\_e.swControlType\_Label, "Label", swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_LeftEdge, options, "")

            'Add a slider
            pm\_Slider = pm\_Group.**AddControl2**(SliderID, swPropertyManagerPageControlType\_e.swControlType\_Slider, "Slider", swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_LeftEdge, options, "Slide")

            'Add a radio button
            pm\_Radio = pm\_Group.**AddControl2**(RadioID, swPropertyManagerPageControlType\_e.swControlType\_Option, "Radio button", swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_LeftEdge, options, "Select")

            'Add a number box
            pm\_Number = pm\_Group.**AddControl2**(NumberID, swPropertyManagerPageControlType\_e.swControlType\_Numberbox, "Number box", swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_LeftEdge, options, "Spin")

            'Add a button
            pm\_Button = pm\_Group.**AddControl2**(ButtonID, swPropertyManagerPageControlType\_e.swControlType\_Button, "Button", swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_LeftEdge, options, "Click")

            'Add a bitmap button
            pm\_BMPButton = pm\_Group.**AddControl2**(BMPButtonID, swPropertyManagerPageControlType\_e.swControlType\_BitmapButton, "Bitmap button", swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_LeftEdge, options, "Click")
            pm\_BMPButton.**SetStandardBitmaps**(swPropertyManagerPageBitmapButtons\_e.swBitmapButtonImage\_parallel)

            'Add a bitmap
            pm\_Bitmap = pm\_Group.**AddControl2**(BitmapID, swPropertyManagerPageControlType\_e.swControlType\_Bitmap, "Bitmap", swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_LeftEdge, options, "Bitmap")
            pm\_Bitmap.**SetStandardBitmap**(swBitmapControlStandardTypes\_e.swBitmapControl\_Volume)

            'Add an ActiveX control
            pm\_ActiveX = pm\_Group.**AddControl2**(ActiveXID, swPropertyManagerPageControlType\_e.swControlType\_ActiveX, "ActiveX", swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_LeftEdge, options, "ActiveX control tip")
            pm\_ActiveX.**SetClass**("*ClassID*", "*LicenseKey*")

        Else

            MsgBox("An
error occurred while attempting to create the PropertyManager Page", vbCritical)

        End
If

    End
Sub

    Public
Sub AfterActivation() Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**AfterActivation**

    End
Sub

    Public
Sub AfterClose() Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**AfterClose**

    End
Sub

    Public
Function OnActiveXControlCreated(ByVal Id As Integer, ByVal Status As
Boolean) As Integer Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnActiveXControlCreated** Debug.Print("ActiveX control
created")

    End
Function

    Public
Sub OnButtonPress(ByVal Id As Integer) Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnButtonPress** Debug.Print("Button clicked")

    End
Sub

    Public
Sub OnCheckboxCheck(ByVal Id As Integer, ByVal Checked As Boolean) Implements
SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnCheckboxCheck**

    End
Sub

    Public
Sub OnClose(ByVal Reason As Integer) Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.OnClose

        If
Reason = swPropertyManagerPageCloseReasons\_e.swPropertyManagerPageClose\_Cancel
Then

            'Cancel
button clicked

            ClickedCancel
= True

        ElseIf
Reason = swPropertyManagerPageCloseReasons\_e.swPropertyManagerPageClose\_Okay
Then

            'OK
button clicked

            ClickedCancel
= False

        End
If

    End
Sub

    Public
Sub OnComboboxEditChanged(ByVal Id As Integer, ByVal Text As String) Implements
SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnComboboxEditChanged**

    End
Sub

    Public
Sub OnComboboxSelectionChanged(ByVal Id As Integer, ByVal Item As Integer)
Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnComboboxSelectionChanged**

    End
Sub

    Public
Sub OnGainedFocus(ByVal Id As Integer) Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.OnGainedFocus

        Dim
varArray As Object

        Debug.Print("Control
box " & Id & " gained focus")

        varArray
= pm\_List.GetSelectedItems

        pm\_Combo.CurrentSelection = varArray(0)

    End
Sub

    Public
Sub OnGroupCheck(ByVal Id As Integer, ByVal Checked As Boolean) Implements
SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnGroupCheck**

    End
Sub

    Public
Sub OnGroupExpand(ByVal Id As Integer, ByVal Expanded As Boolean) Implements
SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnGroupExpand**

    End
Sub

    Public
Function OnHelp() As Boolean Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnHelp**

    End
Function

    Public
Function OnKeystroke(ByVal Wparam As Integer, ByVal Message As Integer,
ByVal Lparam As Integer, ByVal Id As Integer) As Boolean Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnKeystroke**

    End
Function

    Public
Sub OnListboxSelectionChanged(ByVal Id As Integer, ByVal Item As Integer)
Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnListboxSelectionChanged**

    End
Sub

    Public
Sub OnLostFocus(ByVal Id As Integer) Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.OnLostFocus

        Debug.Print("Control
box " & Id & " lost focus")

    End
Sub

    Public
Function OnNextPage() As Boolean Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnNextPage**

    End
Function

    Public
Sub OnNumberboxChanged(ByVal Id As Integer, ByVal Value As Double) Implements
SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnNumberboxChanged**
        Debug.Print("Number box changed")

    End
Sub

    Public
Sub OnOptionCheck(ByVal Id As Integer) Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnOptionCheck**   Debug.Print ("Option selected")

    End
Sub

    Public
Sub OnPopupMenuItem(ByVal Id As Integer) Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnPopupMenuItem**

    End
Sub

    Public
Sub OnPopupMenuItemUpdate(ByVal Id As Integer, ByRef retval As Integer)
Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnPopupMenuItemUpdate**

    End
Sub

    Public
Function OnPreview() As Boolean Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnPreview**

    End
Function

    Public
Function OnPreviousPage() As Boolean Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnPreviousPage**

    End
Function

    Public
Sub OnRedo() Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnRedo**

    End
Sub

    Public
Sub OnSelectionboxCalloutCreated(ByVal Id As Integer) Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnSelectionboxCalloutCreated**

    End
Sub

    Public
Sub OnSelectionboxCalloutDestroyed(ByVal Id As Integer) Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnSelectionboxCalloutDestroyed**

    End
Sub

    Public
Sub OnSelectionboxFocusChanged(ByVal Id As Integer) Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.OnSelectionboxFocusChanged

        Debug.Print("The
focus moved to selection box " & Id)

    End
Sub

    Public
Sub OnSelectionboxListChanged(ByVal Id As Integer, ByVal Count As Integer)
Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.OnSelectionboxListChanged

        pm\_Page.SetCursor(swPropertyManagerPageCursors\_e.swPropertyManagerPageCursors\_Advance)

        Debug.Print("The
list in selection box " & Id & " changed")

    End
Sub

    Public
Sub OnSliderPositionChanged(ByVal Id As Integer, ByVal Value As Double)
Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnSliderPositionChanged** Debug.Print("Slider position
changed")

    End
Sub

    Public
Sub OnSliderTrackingCompleted(ByVal Id As Integer, ByVal Value As Double)
Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnSliderTrackingCompleted**

    End
Sub

    Public
Function OnSubmitSelection(ByVal Id As Integer, ByVal Selection As Object,
ByVal SelType As Integer, ByRef ItemText As String) As Boolean Implements
SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.OnSubmitSelection

        Return True

    End
Function

    Public
Function OnTabClicked(ByVal Id As Integer) As Boolean Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnTabClicked**

    End
Function

    Public
Sub OnTextboxChanged(ByVal Id As Integer, ByVal Text As String) Implements
SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnTextboxChanged**

    End
Sub

    Public
Sub OnUndo() Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnUndo**

    End
Sub

    Public
Sub OnWhatsNew() Implements SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnWhatsNew**

    End
Sub

    Public Sub OnListBoxRMBUp(ByVal Id As Integer,
ByVal posX As Integer, ByVal posY As Integer) Implements
SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnListboxRMBUp**

    End Sub

Public Function OnWindowFromHandleControlCreated(ByVal Id As Integer, ByVal
Status As Boolean) As Integer Implements
SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnWindowFromHandleControlCreated**

    End Function

    Public Sub OnNumberBoxTrackingCompleted(ByVal Id As Integer,
ByVal Value As Double) Implements
SolidWorks.Interop.swpublished.IPropertyManagerPage2Handler9.**OnNumberBoxTrackingCompleted**

    End Sub

End Class

[Back to top](#Top)