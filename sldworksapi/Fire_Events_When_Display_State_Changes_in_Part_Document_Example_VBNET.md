<!-- source: sldworksapi/Fire_Events_When_Display_State_Changes_in_Part_Document_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Fire Events When Display State Changes in Part Document Example (VB.NET)

This example shows how to fire the events related to changing display
states of a configuration in a part document.

'---------------------------------------------------------------

' Preconditions:

' 1. Open a part document that has

'    a
configuration with multiple display states.

' 2. Run this macro in debug mode.

' 3. Change the display state of the
active configuration in SOLIDWORKS

'    (click
the ConfigurationManager tab and double-click

'    a
different display state).

'

' Postcondition: A message box is displayed informing

' you
that the display state is about change.
After the display state changes,

' another
message box is displayed informing
you that the display

' state
has changed.

'---------------------------------------------------------------

Option Explicit On

Imports SolidWorks.Interop.sldworks

Imports SolidWorks.Interop.swconst

Imports System

Imports System.Diagnostics

Imports System.Collections

Partial Class SolidWorksMacro

    Public
WithEvents swPart As PartDoc

    Public
Sub Main()

        Dim
swModel As ModelDoc2

        Dim
openPart As Hashtable

        swModel
= swApp.ActiveDoc

        'Set
up events

        swPart
= swModel

        openPart
= New Hashtable

        AttachEventHandlers()

    End
Sub

    Sub
AttachEventHandlers()

        AttachSWEvents()

    End
Sub

    Sub
AttachSWEvents()

        AddHandler
swPart.ActiveDisplayStateChangePreNotify, AddressOf Me.swPart\_ActiveDisplayStateChangePreNotify

        AddHandler
swPart.ActiveDisplayStateChangePostNotify, AddressOf Me.swPart\_ActiveDisplayStateChangePostNotify

    End
Sub

    Private
Function swPart\_ActiveDisplayStateChangePreNotify()
As Integer

        'Send
message when user changes display state in the ConfigurationManager

        MsgBox("The
active configuration's display state is about to change.")

    End
Function

    Private
Function swPart\_ActiveDisplayStateChangePostNotify(ByVal
DisplayStateName As String) As Integer

        'Send
message after user changes display state in the ConfigurationManager

        MsgBox("The
active configuration's display state has changed.")

    End
Function

    '''
<summary>

    '''
The SldWorks swApp variable is pre-assigned for you.

    '''
</summary>

    Public
swApp As SldWorks

End Class