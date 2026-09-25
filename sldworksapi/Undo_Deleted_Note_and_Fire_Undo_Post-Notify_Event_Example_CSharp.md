<!-- source: sldworksapi/Undo_Deleted_Note_and_Fire_Undo_Post-Notify_Event_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Undo Deleted Note and Fire Undo Pre- and Post-Notify Events Example (C#)

This example demonstrates firing Undo pre- and post-notification events
in a drawing document.

//---------------------------------------------------------------------------
// Preconditions: Open *public\_documents***\samples\tutorial\AutoCAD\7550-021.slddrw**.
//
// Postconditions:
// 1. Selects and deletes the note in **Drawing View1**.
// 2. Undoes the deleted note.
// 3. Fires pre-notification event indicating that an undo action is about to

//    occur and fires post-notification event indicating that an
undo
//    action occurred.
// 4. Click **OK** to close each message box.
//
// NOTE: Because the drawing is used elsewhere, do not save changes.
//---------------------------------------------------------------------------

using SolidWorks.Interop.sldworks;

using SolidWorks.Interop.swconst;

using System;

using System.Collections;

using System.Windows.Forms;

namespace UndoPostNotifyDrawingCSharp.csproj

{

partial class SolidWorksMacro

{

    public
DrawingDoc swDrawing;

    public
void Main()

    {

        ModelDoc2
swModel = default(ModelDoc2);

        ModelDocExtension
swModelDocExt = default(ModelDocExtension);

        bool
boolstatus = false;

        Hashtable
openDrawing = default(Hashtable);

        swModel
= (ModelDoc2)swApp.ActiveDoc;

        swModelDocExt
= (ModelDocExtension)swModel.Extension;

        //
Event notification

        swDrawing
= (DrawingDoc)swModel;

        openDrawing
= new Hashtable();

        AttachEventHandlers();

        //
Activate the drawing view that contains

        //
the note you want to delete

        boolstatus
= swDrawing.ActivateView("Drawing
View3");

        boolstatus
= swModelDocExt.SelectByID2("DetailItem77@Drawing
View3", "NOTE", 0.3058741216774, 0.1870419466786, 0, false,
0, null, 0);

        //
Delete the selected note

        swModel.EditDelete();

        //
Undo deletion of note

        swModel.EditUndo2(1);

        //
Post-notification is fired

        //
Rebuild the drawing

        swModel.ForceRebuild3(true);

    }

    public
void AttachEventHandlers()

    {

        AttachSWEvents();

    }

    public
void AttachSWEvents()

    {

        swDrawing.**UndoPostNotify**
+= this.swDrawing\_UndoPostNotify;

        swDrawing.**UndoPreNotify**
+= this.swDrawing\_UndoPreNotify;

    }

    private
int swDrawing\_UndoPostNotify()

    {

        //
Display message after Undo

        //
NOTE: Because the message box may be displayed

        //
behind an opened window, you might not see it.

        //
If so, then check the Taskbar.

        MessageBox.Show("An
undo post-notification event has been fired.");

        return
1;

    }

    private
int b()

    {

        //
Display message after Undo

        //
NOTE: Because the message box may be displayed

        //
behind an opened window, you might not see it.

        //
If so, then check the Taskbar.

        MessageBox.Show("An
Undo pre-notification event has been fired.");

        return
1;

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