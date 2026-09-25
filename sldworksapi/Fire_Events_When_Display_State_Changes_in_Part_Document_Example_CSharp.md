<!-- source: sldworksapi/Fire_Events_When_Display_State_Changes_in_Part_Document_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Fire Events When Display State Changes in Part Document (C#)

This example shows how to fire the events related to changing display
states of a configuration in a part document.

//---------------------------------------------------------------

// Preconditions:

// 1. Open a part document that has

//    a
configuration with multiple display states.

// 2. Run this macro in debug mode.

// 3. Change the display state of the
active configuration in SOLIDWORKS

//    (click
the ConfigurationManager tab and double-click

//    a
different display state).

//

// Postcondition: A message box is displayed informing

// you
that the display state is about change.
After the display state changes,

// another
message box is displayed informing
you that the display

// state
has changed.

//---------------------------------------------------------------

using SolidWorks.Interop.sldworks;

using SolidWorks.Interop.swconst;

using System;

using System.Collections;

using System.Windows.Forms;

namespace FireEventsWhenDisplayStateChangesCSharp.csproj

{

    public
partial class SolidWorksMacro

    {

        public
PartDoc swPart;

        public
void Main()

        {

            ModelDoc2
swModel;

            Hashtable
openPart;

            swModel
= (ModelDoc2)swApp.ActiveDoc;

            //Set
up events

            swPart
= (PartDoc)swModel;

            openPart
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

            swPart.ActiveDisplayStateChangePreNotify
+= this.swPart\_ActiveDisplayStateChangePreNotify;

            swPart.ActiveDisplayStateChangePostNotify
+= this.swPart\_ActiveDisplayStateChangePostNotify;

        }

        public
int swPart\_ActiveDisplayStateChangePreNotify()

        //Send
message when user changes display state in the ConfigurationManager

        {

            MessageBox.Show("The
active configuration's display state is about to change.");

            return
1;

        }

        public
int swPart\_ActiveDisplayStateChangePostNotify(string
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