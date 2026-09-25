<!-- source: sldworksapiprogguide/Overview/Connect_to_SolidWorks_Message_Pump_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Connect to SOLIDWORKS Message Pump to Handle Keystrokes and Accelerator Keys (C#)

This example shows how to connect to a SOLIDWORKS message pump by creating,
installing, and uninstalling a hook for a modeless dialog box or PropertyManager
page for intercepting keystrokes and handling accelerator keys.

//Create, install, and uninstall a hook for a modeless
dialog box

//or PropertyManager page for intercepting keystrokes
and

//handling accelerator keys

using System;

using System.Runtime.InteropServices;

namespace WinHooks

{

    public
class HookEventArgs : EventArgs

    {

        public
int HookCode;    //
Hook code

        public
IntPtr wParam;   //
WPARAM argument

        public
IntPtr lParam;   //
LPARAM argument

    }

    //
Hook Types

    public
enum HookType : int

    {

        WH\_JOURNALRECORD
= 0,

        WH\_JOURNALPLAYBACK
= 1,

        WH\_KEYBOARD
= 2,

        WH\_GETMESSAGE
= 3,

        WH\_CALLWNDPROC
= 4,

        WH\_CBT
= 5,

        WH\_SYSMSGFILTER
= 6,

        WH\_MOUSE
= 7,

        WH\_HARDWARE
= 8,

        WH\_DEBUG
= 9,

        WH\_SHELL
= 10,

        WH\_FOREGROUNDIDLE
= 11,

        WH\_CALLWNDPROCRET
= 12,

        WH\_KEYBOARD\_LL
= 13,

        WH\_MOUSE\_LL
= 14

    }

    public
class LocalWindowsHook

    {

        //
Filter function delegate

        public
delegate int HookProc(int code, IntPtr wParam,

           IntPtr
lParam);

        //
Internal properties

        protected
IntPtr m\_hhook = IntPtr.Zero;

        protected
HookProc m\_filterFunc = null;

        protected
HookType m\_hookType;

        //
Event delegate

        public
delegate void HookEventHandler(object sender, HookEventArgs e);

        //
Event: HookInvoked

        public
event HookEventHandler HookInvoked;

        protected
void OnHookInvoked(HookEventArgs e)

        {

            if
(HookInvoked != null)

                HookInvoked(this,
e);

        }

        //
Class constructor(s)

        public
LocalWindowsHook(HookType hook)

        {

            m\_hookType
= hook;

            m\_filterFunc
= new HookProc(this.CoreHookProc);

        }

        public
LocalWindowsHook(HookType hook, HookProc func)

        {

            m\_hookType
= hook;

            m\_filterFunc
= func;

        }

        //
Default filter function

        public
int CoreHookProc(int code, IntPtr wParam, IntPtr lParam)

        {

            if
(code < 0)

                return
CallNextHookEx(m\_hhook, code, wParam, lParam);

            //
Let clients determine what to do

            HookEventArgs
e = new HookEventArgs();

            e.HookCode
= code;

            e.wParam
= wParam;

            e.lParam
= lParam;

            OnHookInvoked(e);

            //
Yield to the next hook in the chain

            return
CallNextHookEx(m\_hhook, code, wParam, lParam);

        }

        //
Install the hook

        public
void Install()

        {

            m\_hhook
= SetWindowsHookEx(

                m\_hookType,

                m\_filterFunc,

                IntPtr.Zero,

                (int)
AppDomain.GetCurrentThreadId());

        }

        //
Uninstall the hook

        public
void Uninstall()

        {

            UnhookWindowsHookEx(m\_hhook);

        }

        #region
Win32 Imports

        //
Win32: SetWindowsHookEx()

        [DllImport("user32.dll")]

        protected
static extern IntPtr SetWindowsHookEx(HookType code,

            HookProc
func,

            IntPtr
hInstance,

            int
threadID);

        //
Win32: UnhookWindowsHookEx()

        [DllImport("user32.dll")]

        protected
static extern int UnhookWindowsHookEx(IntPtr hhook);

        //
Win32: CallNextHookEx()

        [DllImport("user32.dll")]

        protected
static extern int CallNextHookEx(IntPtr hhook,

            int
code, IntPtr wParam, IntPtr lParam);

        #endregion

    }

}