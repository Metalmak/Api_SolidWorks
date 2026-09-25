<!-- source: sldworksapi/Fire_Events_When_Display_State_Changes_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Fire Events When Display State Changes Example (C#)

This example shows how to fire the events related to changing display
states of a configuration in an assembly document.

```
//---------------------------------------------------------------
// Preconditions:
// 1. Open an assembly document that has a configuration with multiple
//    display states.
// 2. Run this macro in debug mode.
// 3. Change the display state of the active configuration in SOLIDWORKS
//    (click the ConfigurationManager tab and double-click
//    a different display state).
//
// Postconditions:
// 1. Displays a message box informing you that the display state is about to
//    change.
// 2. After the display state changes, displays another message informing you
//    that the display state has changed.
//
// NOTE: This example also fires these events when you change
// configurations in an assembly document.
//---------------------------------------------------------------
using SolidWorks.Interop.sldworks;
using SolidWorks.Interop.swconst;
using System;
using System.Collections;
using System.Windows.Forms;

namespace Macro1.csproj
{
    public
 partial class SolidWorksMacro
```

    {

        public
AssemblyDoc swAssem;
        public
void Main()

        {

            ModelDoc2
swModel;
            Hashtable
openAssem;
            swModel
= (ModelDoc2)swApp.ActiveDoc;

            //Set
up events
            swAssem
= (AssemblyDoc)swModel;
            openAssem
= new Hashtable();
            AttachEventHandlers();

        }

        ///
<summary>
        ///
 The SldWorks
swApp variable is pre-assigned for you.
        ///
</summary>
        public
SldWorks swApp;

        public
void AttachEventHandlers()
        {
            AttachSWEvents();
        }

        public
void AttachSWEvents()
        {
            swAssem.**ActiveDisplayStateChangePreNotify** +=
this.swAssem\_ActiveDisplayStateChangePreNotify;
            swAssem.**ActiveDisplayStateChangePostNotify** +=
this.swAssem\_ActiveDisplayStateChangePostNotify;
        }

        public
int swAssem\_ActiveDisplayStateChangePreNotify()
        //Send
message when user changes display state in the ConfigurationManager
        {
            MessageBox.Show("The
active configuration's display state is about to change.");
            return
1;
        }

        public
int swAssem\_ActiveDisplayStateChangePostNotify(string
DisplayStateName)
        //Send
message after user changes display state in the ConfigurationManager
        {
            MessageBox.Show("The
active configuration's display state has changed.");
            return
1;
        }

    }
}