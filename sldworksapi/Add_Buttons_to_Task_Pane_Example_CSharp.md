<!-- source: sldworksapi/Add_Buttons_to_Task_Pane_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Add Buttons to Task Pane Example (C#)

This example shows how to add standard SOLIDWORKS and custom buttons to the
Task Pane.

//-----------------------------------------------------------------------
// 1. Copy **save.png** from *public\_documents***\samples\tutorial\api** to
this macro's
//    **SwMacro** folder.
// 2. Clear the **Stop VSTA debugger on macro exit** check box if selected

//    in **Tools > Options > System Options**.
// 3. Open the Immediate window.
//
// Postconditions:
// 1. Opens the Task Pane and loads the **My Calendar** control with
//    the specified standard and custom buttons at the
//    top of the pane.
// 2. Click each button from left to right and examine the Immediate
//    window after each click.
// 3. Click the **Stop Debugging** button in the IDE.
// 4. Select the **Stop VSTA debugger on macro exit** check box in
//    **Tools > Options > System Options** if cleared in
//    Preconditions step 2.
//----------------------------------------------------------------------
using
SolidWorks.Interop.sldworks;
using
SolidWorks.Interop.swconst;
using System;
using System.Collections;
using System.Windows.Forms;
using System.Diagnostics;

namespace
Macro1CSharp.csproj
{
    partial
class
SolidWorksMacro
    {

        public TaskpaneView
swTaskPane;
        public
int buttonIdx;

        public
void Main()
        {

            bool result =
false;
            string folder =
null;
            string bitmap =
null;
            string toolTip
= null;
            string ctrlName
= null;
            string
ctrlLicKey = null;

            folder = swApp.**GetCurrentMacroPathFolder**() +
"\\";

            // Use default image for Task Pane tab

            bitmap = "";
            toolTip = "My Calendar";
            ctrlName = "My.Calendar";
            ctrlLicKey = "";
            swTaskPane = (TaskpaneView)swApp.**CreateTaskpaneView2**(bitmap,
toolTip);

            // Add standard and custom buttons to
Task Pane
            result = swTaskPane.**AddCustomButton**(folder +
"save.png",
"Save (custom png)");
            result = swTaskPane.**AddStandardButton**((int)swTaskPaneBitmapsOptions\_e.swTaskPaneBitmapsOptions\_Next,
"Next (standard)");
            result = swTaskPane.**AddStandardButton**((int)swTaskPaneBitmapsOptions\_e.swTaskPaneBitmapsOptions\_Back,
"Back (standard)");
            result = swTaskPane.**AddStandardButton**((int)swTaskPaneBitmapsOptions\_e.swTaskPaneBitmapsOptions\_Ok,
"OK (standard)");
            result = swTaskPane.**AddStandardButton**((int)swTaskPaneBitmapsOptions\_e.swTaskPaneBitmapsOptions\_Close,
"Close (standard)");

            // Add control to Task Pane for the
buttons
            swTaskPane.**AddControl**(ctrlName,
ctrlLicKey);

            // Set up events

            AttachEventHandlers();
        }

        public
void AttachEventHandlers()
        {
            AttachSWEvents();
        }

        public
void AttachSWEvents()
        {
            swTaskPane.TaskPaneActivateNotify += this.swTaskPane\_TaskPaneActivateNotify;
            swTaskPane.TaskPaneDestroyNotify += this.swTaskPane\_TaskPaneDestroyNotify;
            swTaskPane.TaskPaneToolbarButtonClicked +=
this.swTaskPane\_TaskPaneToolbarButtonClicked;
        }

        public
int swTaskPane\_**TaskPaneActivateNotify**()
        {
            if (swTaskPane.**GetButtonState**(0)
== false)
            {
                for (buttonIdx
= 0; buttonIdx <= 20; buttonIdx++)
                {
                    swTaskPane.**SetButtonState**(buttonIdx,
true);
                }
            }
            else
            {
                for (buttonIdx
= 0; buttonIdx <= 20; buttonIdx++)
                {
                    swTaskPane.**SetButtonState**(buttonIdx,
false);
                }
            }
            return 0;
        }

        public
int swTaskPane\_**TaskPaneDestroyNotify**()
        {
            MessageBox.Show("Remove control from
Task Pane?");
            return 1;
        }

        public
int swTaskPane\_**TaskPaneToolbarButtonClicked**(int
ButtonIndex)
        {
            switch ((ButtonIndex
+ 1))
            {
                case
1:
                    Debug.Print("Save (custom
png) button clicked.");
                    break;
                case
2:
                    Debug.Print("Next button
clicked.");
                    break;
                case
3:
                    Debug.Print("Back button
clicked.");
                    break;
                case
4:
                    Debug.Print("Okay button
clicked.");
                    break;
                case
5:
                    Debug.Print("Close button
clicked and tab deleted.");
                    swTaskPane.**DeleteView**();
                    break;
            }
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