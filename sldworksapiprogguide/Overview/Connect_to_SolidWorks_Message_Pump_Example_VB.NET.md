<!-- source: sldworksapiprogguide/Overview/Connect_to_SolidWorks_Message_Pump_Example_VB.NET.htm -->

# SOLIDWORKS API Help

# Connect to SOLIDWORKS Message Pump to Handle Keystrokes and Accelerator Keys (VB.NET)

This example shows how to connect to a SOLIDWORKS message pump by creating,
installing, and uninstalling a hook for a modeless dialog box or PropertyManager
page for intercepting keystrokes and handling accelerator keys.

' Create, install, and uninstall a hook for a modeless
dialog box

' or PropertyManager page for intercepting keystrokes
and

' handling accelerator keys

Imports System

Imports System.Runtime.InteropServices

Namespace WinHooks

    Public
Class HookEventArgs

        Inherits
EventArgs

        Public
HookCode As Integer   '
Hook code

        Public
wParam As IntPtr   '
WPARAM argument

        Public
lParam As IntPtr  '
LPARAM argument

    End
Class

    '
Hook Types

    Public
Enum HookType

        WH\_JOURNALRECORD
= 0

        WH\_JOURNALPLAYBACK
= 1

        WH\_KEYBOARD
= 2

        WH\_GETMESSAGE
= 3

        WH\_CALLWNDPROC
= 4

        WH\_CBT
= 5

        WH\_SYSMSGFILTER
= 6

        WH\_MOUSE
= 7

        WH\_HARDWARE
= 8

        WH\_DEBUG
= 9

        WH\_SHELL
= 10

        WH\_FOREGROUNDIDLE
= 11

        WH\_CALLWNDPROCRET
= 12

        WH\_KEYBOARD\_LL
= 13

        WH\_MOUSE\_LL
= 14

    End
Enum

    Public
Class LocalWindowsHook

        '
Filter function delegate

        Public
Delegate Function HookProc(ByVal code As Integer, ByVal wParam As IntPtr,
ByVal lParam As IntPtr) As Integer

        '
Internal properties

        Protected
m\_hhook As IntPtr = IntPtr.Zero

        Protected
m\_filterFunc As HookProc = Nothing

        Protected
m\_hookType As HookType

        '
Event delegate

        Public
Delegate Sub HookEventHandler(ByVal sender As Object, ByVal e As HookEventArgs)

        '
Event: HookInvoked

        Public
Event HookInvoked As HookEventHandler

        Protected
Sub OnHookInvoked(ByVal e As HookEventArgs)

            RaiseEvent
HookInvoked(Me, e)

        End
Sub

        '
Class constructor(s)

        Public
Sub New(ByVal hook As HookType)

            m\_hookType
= hook

            m\_filterFunc
= New HookProc(AddressOf Me.CoreHookProc)

        End
Sub

        Public
Sub New(ByVal hook As HookType, ByVal func As HookProc)

            m\_hookType
= hook

            m\_filterFunc
= func

        End
Sub

        '
Default filter function

        Public
Function CoreHookProc(ByVal code As Integer, ByVal wParam As IntPtr, ByVal
lParam As IntPtr) As Integer

            If
code < 0 Then Return CallNextHookEx(m\_hhook, code, wParam, lParam)

            '
Let clients determine what to do

            Dim
e As HookEventArgs = New HookEventArgs()

            e.HookCode
= code

            e.wParam
= wParam

            e.lParam
= lParam

            OnHookInvoked(e)

            '
Yield to the next hook in the chain

            CoreHookProc
= CallNextHookEx(m\_hhook, code, wParam, lParam)

        End
Function

        '
Install the hook

        Public
Sub Install()

            m\_hhook
= SetWindowsHookEx(m\_hookType, m\_filterFunc, IntPtr.Zero, AppDomain.GetCurrentThreadId())

        End
Sub

        '
Uninstall the hook

        Public
Sub Uninstall()

            UnhookWindowsHookEx(m\_hhook)

        End
Sub

        '
Win32 Imports

        '
Win32: SetWindowsHookEx()

        Declare
Function SetWindowsHookEx Lib "user32" Alias "SetWindowsHookExA"
(ByVal code As HookType, ByVal func As HookProc, ByVal hInstance As IntPtr,
ByVal threadID As Integer) As Integer

        '
Win32: UnhookWindowsHookEx()

        Declare
Function UnhookWindowsHookEx Lib "user32" (ByVal hhook As IntPtr)
As Integer

        '
Win32: CallNextHookEx()

        Declare
Function CallNextHookEx Lib "user32" (ByVal hhook As IntPtr,
ByVal code As Integer, ByVal wParam As IntPtr, ByVal lParam As IntPtr)
As Integer

    End
Class

End Namespace