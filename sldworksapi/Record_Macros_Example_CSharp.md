<!-- source: sldworksapi/Record_Macros_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Record Macros Example (C#)

This example shows how to add
two lines to a macro recording.

//---------------------------------------------------------------------------

// Preconditions:

// 1.
Add a reference to **SolidWorks.Interop.swcommands.dll**.

//
// Postconditions:

// 1.
Displays a message box informing you that
//    macro recording has started. Click **OK**.
// 2. Displays the Save asdialog.
//
3. Type **Macro2** in **File name** and
select the languages
//    to which to save macros in **Save as type**.
// 4. Writes two lines of text to the macros in the languages
//    corresponding to the **Save as type** you selected.
// 5. Displays a message box informing you that
//    macro recording has ended. Click **OK**.
// 6. Displays a message box asking you if you
//    want to stop debugging. Click **Yes**.
// 7. Run the just-recorded macros to verify.
//--------------------------------------------------------------------------
using
SolidWorks.Interop.sldworks;
using
SolidWorks.Interop.swconst;
using
SolidWorks.Interop.swcommands;
using System;
using System.Windows.Forms;

namespace
RecordLineCSharpSldWorksCSharp.csproj
{

    partial
class
SolidWorksMacro
    {

        public SldWorks
swAppEvents;

        public
void Main()
        {

            // Set up events
            swAppEvents = (SldWorks)swApp;
            AttachEventHandlers();

            // Start macro recording
            swApp.**RunCommand**((int)swCommands\_e.swCommands\_RecordPauseMacro,
"");

            // Write to VBA macro
            swApp.**RecordLine**("'
Test");
            swApp.**RecordLine**("MsgBox(\"C:\\Test\\\")");

            // Write to C# macro
            swApp.**RecordLineCSharp**("//
Test");
            swApp.**RecordLineCSharp**("System.Windows.Forms.MessageBox.Show(\"C:\\\\Test\\\\\");");

            // Write to VB.NET macro
            swApp.**RecordLineVBnet**("'
Test");
            swApp.**RecordLineVBnet**("MsgBox(\"C:\\Test\\\")");

            //Stop the
macro recordings

            swApp.**RunCommand**((int)swCommands\_e.swCommands\_StopMacro,
"");
        }

        public
void AttachEventHandlers()
        {
            AttachSWEvents();
        }

        public
void AttachSWEvents()
        {
            swAppEvents.BeginRecordNotify += this.swAppEvents\_BeginRecordNotify;
            swAppEvents.EndRecordNotify += this.swAppEvents\_EndRecordNotify;
        }

        private
int swAppEvents\_**BeginRecordNotify**()
        {
            //Send message when the macro recording
starts
            MessageBox.Show("Macro
recording starting.");
            return 1;
        }

        private
int swAppEvents\_**EndRecordNotify**()
        {
            //Send message when macro recording ends

            MessageBox.Show("Macro
recording ended.");
            return 1;
        }

        ///
<summary>
        ///
The SldWorks swApp variable is pre-assigned for you.
        ///
</summary>
        public
SldWorks swApp;

    }
}