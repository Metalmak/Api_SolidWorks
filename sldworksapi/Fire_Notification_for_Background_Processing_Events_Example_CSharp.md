<!-- source: sldworksapi/Fire_Notification_for_Background_Processing_Events_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Fire Notifications for Background Processing Events Example (C#)

This example shows how to fire notifications when background processing
events occur.

//----------------------------------------------------------------------------
// Preconditions:
//  1. Create a VSTA C# macro.
//     a. Copy and paste [SolidWorksMacro.cs](#SolidWorksMacro) code in the macro.

//     b. Create a form, Form1, that contains the following
//        controls:
//        \* CheckBox1 with caption **Enable background processing and open**
//          **drawing**.
//        \* button1 with caption **Close after background processing end event**
//          **fires**".
//     c. Copy and paste [Form1.cs](#Form1) code in your form's code window.

//     d. Modify the path in Form1.cs to open a huge drawing document that
//        contains many parts.
//  2. Press F5 to start and close the debugger.
//  3. Click **Build > Build***macro\_name* to build a DLL for the macro.
//  4. Save and close the macro.
//
// Postconditions:

//  1. Open the Windows Task manager, click the Processes tab, and click the CPU column

//     header to sort the processes in descending order.
//  2. In SOLIDWORKS, click **Tools > Macro > Run**.
//     a. Locate your macro's **\SwMacro\bin\Debug** folder.
//     b. Select *macro\_name***.dll**.
//     c. Click **Open**
to open the form.
//  3. Select the **Enable background processing and open drawing** checkbox on the form.
//  4. Displays a checkmark in the check box.
//  5. Click **OK** to close the **Background processing enabled** message box.
//  6. Opens the specified drawing.
//  7. Fires the background processing start events.
//  8. Click **OK** to close the **Background processing start event fired** message box.

//  9. In the Windows Task Manager, observe that several **sldbgproc.exe** processes are
//     occupying most of the CPU.
// 10. Click **OK** to close the **Background processing stop event fired** message box.
// 11. Click **Close after background processing end event fired** button on the form.
// 12. Unloads Form1.

//----------------------------------------------------------------------------------

//SolidWorksMacro.cs

using SolidWorks.Interop.sldworks;
using System.Runtime.InteropServices;
using System;
using System.Windows.Forms;

namespace BackgroundProcessingEventsCSharp.csproj
{

    public partial class SolidWorksMacro
    {
        public SldWorks swApp;

        public void Main()
        {
            //Create and show an instance of the form
            Form1 myForm = new Form1();
            myForm.Show();

        }

    }
}

//Form1

using SolidWorks.Interop.sldworks;
using SolidWorks.Interop.swconst;
using System.Windows.Forms;
using System.Diagnostics;
using System.Collections;
using System.Runtime.InteropServices;
using System;
using System.ComponentModel;
using System.Data;
using System.Drawing;
using System.Text;

namespace BackgroundProcessingEventsCSharp.csproj
{
    public partial class Form1 : Form
    {
        public Form1()
        {
            InitializeComponent();
        }

        public SldWorks swApp;
        public bool checkBoxClicked;

        private void checkBox1\_CheckedChanged(object sender, EventArgs e)
        {

            try
            {
                swApp = (SldWorks)System.Runtime.InteropServices.Marshal.GetActiveObject("SldWorks.Application");
            }
            catch (Exception ex)
            {
                MessageBox.Show(ex.Message);
                return;
            }

            ModelDoc2 swModelDoc = default(ModelDoc2);
            DrawingDoc swDrawingDoc = default(DrawingDoc);

            string filePath = null;
            filePath = "*path\_and\_filename\_of\_huge\_drawing*";

            DocumentSpecification docSpecification = default(DocumentSpecification);

            // Set up events
            AttachEventHandlers();

            // Enable background processing
            swApp.**EnableBackgroundProcessing** = true;
            MessageBox.Show("Background processing enabled");

            // Open huge drawing
            docSpecification = (DocumentSpecification)swApp.**GetOpenDocSpec**(filePath);
            docSpecification.**Silent** = true;
            swModelDoc = (ModelDoc2)swApp.**OpenDoc7**(docSpecification);

            swDrawingDoc = (DrawingDoc)swModelDoc;

            // Set document background processing to application setting
            swDrawingDoc.**BackgroundProcessingOption** = (int)swBackgroundProcessOption\_e.swBackgroundProcessing\_DeferToApplication;

        }

        public void AttachEventHandlers()
        {
            AttachSWEvents();
        }

        public void AttachSWEvents()
        {
            swApp.**BackgroundProcessingStartNotify** += this.mySwApp\_BackgroundProcessingStartNotify;
            swApp.**BackgroundProcessingEndNotify** += this.mySwApp\_BackgroundProcessingEndNotify;
        }

        private int mySwApp\_**BackgroundProcessingStartNotify**(string filename)
        {
            MessageBox.Show("Background processing start event fired");
            return 1;
        }
        private int mySwApp\_**BackgroundProcessingEndNotify**(string filename)
        {
            MessageBox.Show("Background processing end event fired");
            swApp.**EnableBackgroundProcessing** = false;
            return 1;
        }
        public void CheckBox1\_Click(object sender, System.EventArgs e)
        {
            checkBoxClicked = true;
        }

        private void button1\_Click(object sender, EventArgs e)
        {
            this.Close();
        }
    }
}