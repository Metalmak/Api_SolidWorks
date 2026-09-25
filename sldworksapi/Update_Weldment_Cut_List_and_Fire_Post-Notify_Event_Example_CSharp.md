<!-- source: sldworksapi/Update_Weldment_Cut_List_and_Fire_Post-Notify_Event_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Update Weldment Cut List and Fire Post-Notify Event Example (C#)

This example shows how to handle the post-notification
event that fires

when the weldment cut list is updated.

//------------------------------------------------------

// Preconditions:

// Specified file to open exists.

//

// Postconditions:

// 1. Right-click on the Cut list folder.

// 2. Select Update from the right-click menu.

// 3. A message box displays (look in the taskbar for
the hidden dialog).

// 4. Click OK.

// 5. Stop the macro (CTRL-ALT-Break).

//------------------------------------------------------

using SolidWorks.Interop.sldworks;

using SolidWorks.Interop.swconst;

using System;

namespace UpdateWeldmentCutListandFirePostNotifyEvent\_CSharp.csproj

{

    partial
class SolidWorksMacro

    {

        public
PartDoc swPart;

        public
void Main()

        {

            swApp.SetUserPreferenceToggle((int)swUserPreferenceToggle\_e.swStopDebuggingVstaOnExit,
false);

            ModelDoc2
swModel = default(ModelDoc2);

            DocumentSpecification
swDocSpecification = default(DocumentSpecification);

            swDocSpecification
= (DocumentSpecification)swApp.GetOpenDocSpec("C:\\Users\\Public\\Documents\\SOLIDWORKS\\SOLIDWORKS 2018\\samples\\tutorial\\weldments\\weldment\_box2.sldprt");

            swDocSpecification.DocumentType
= (int)swDocumentTypes\_e.swDocPART;

            swModel
= swApp.OpenDoc7(swDocSpecification);

            swModel
= (ModelDoc2)swApp.ActiveDoc;

            swPart
= (PartDoc)swModel;

            //
Set up event

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

            swPart.WeldmentCutListUpdatePostNotify += this.swPart\_WeldmentCutListUpdatePostNotify;

        }

        public
int swPart\_WeldmentCutListUpdatePostNotify()

        {

            System.Windows.Forms.MessageBox.Show("The
cut list is updated.");

            swApp.SetUserPreferenceToggle((int)swUserPreferenceToggle\_e.swStopDebuggingVstaOnExit,
true);

            return
0;

        }

        public
SldWorks swApp;

    }

}