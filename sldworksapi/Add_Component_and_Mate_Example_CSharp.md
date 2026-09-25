<!-- source: sldworksapi/Add_Component_and_Mate_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Add and Mate Component Example (C#)

This example shows how to add a component to an assembly and mate it.

//---------------------------------------------------------------------------
// Preconditions:
// 1. Verify that these documents exist in *public\_documents***\samples\tutorial\toolbox**://    \* **lens\_mount.sldasm**//    \* **camtest.sldprt**
// 2. Open the Immediate window.
//
// Postconditions:
// 1. Opens **lens\_mount.sldasm**.
// 2. Adds the specified component, **camtest.sldprt**, to the assembly.
// 3. Fires the **AddItemNotify** event.
// 4. Makes the specified component virtual by saving it to the
//    assembly with
a new name.
// 5. Fires the **RenameItemNotify** event.
// 6. Adds a mate between the selected planes to the assembly.
// 7. Inspect the Immediate window and FeatureManager design tree.
//
// NOTE: Because the models are used elsewhere, do not save changes.
//----------------------------------------------------------------------------

using SolidWorks.Interop.sldworks;
using SolidWorks.Interop.swconst;
using System.Runtime.InteropServices;
using System;
using System.Diagnostics;
using System.Collections;
using System.Windows.Forms;

namespace MakeVirtualCSharp.csproj
{
    partial class SolidWorksMacro
    {

        public AssemblyDoc swAssemblyDoc;
        ModelDoc2 swModel;
        ModelDocExtension swDocExt;
        Hashtable openAssem;
        string tmpPath;
        ModelDoc2 tmpObj;
        bool boolstat;
        bool stat;
        Component2 swComponent;
        Feature matefeature;
        string MateName;
        string FirstSelection;
        string SecondSelection;
        string strCompName;
        string AssemblyTitle;
        string AssemblyName;
        int errors;
        int warnings;
        string
fileName;

        int mateError;

        public void Main()
        {

            // Open assembly
            fileName =

"C:\\Users\\Public\\Documents\\SOLIDWORKS\SOLIDWORKS 2018\\samples\\tutorial\\toolbox\\lens\_mount.sldasm";
            swModel = (ModelDoc2)swApp.**OpenDoc6**(fileName,
(int)swDocumentTypes\_e.swDocASSEMBLY,
(int)swOpenDocOptions\_e.swOpenDocOptions\_Silent,
"",
ref errors,
ref
warnings);

            // Set up event
            swAssemblyDoc = (AssemblyDoc)swModel;
            openAssem = new Hashtable();
            AttachEventHandlers();

            // Get title of assembly document
            AssemblyTitle = swModel.**GetTitle**();

            // Split the title into two strings using the period as the delimiter
            string[] strings = AssemblyTitle.Split(new Char[] { '.' });

            // Use AssemblyName when mating the component with the assembly
            AssemblyName = (string)strings[0];

            Debug.Print("Name of assembly: " + AssemblyName);

            boolstat = true;
            string strCompModelname = null;
            strCompModelname = "camtest.sldprt";

            // Because the component resides in the same folder as the assembly, get
            // the assembly's path and use it when opening the component
            tmpPath = swModel.**GetPathName**();
            int idx;
            idx = tmpPath.LastIndexOf("lens\_mount.sldasm");
            string compPath;
            tmpPath = tmpPath.Substring(0, (idx));
            compPath = string.Concat(tmpPath, strCompModelname);

            // Open the component
            tmpObj = (ModelDoc2)swApp.**OpenDoc6**(compPath, (int)swDocumentTypes\_e.swDocPART, (int)swOpenDocOptions\_e.swOpenDocOptions\_Silent, "", ref errors, ref warnings);

            // Check to see if the file is read-only or cannot be found; display error
            // messages if either
            if (warnings == (int)swFileLoadWarning\_e.swFileLoadWarning\_ReadOnly)
            {
                MessageBox.Show("This file is read-only.");
                boolstat = false;
            }

            if (tmpObj == null)
            {
                MessageBox.Show("Cannot locate the file.");
                boolstat = false;
            }

            // Activate the assembly so that you can add the component to it
            swModel = (ModelDoc2)swApp.**ActivateDoc3**(AssemblyTitle, true, (int)swRebuildOnActivation\_e.swUserDecision, ref errors);

            // Add the part to the assembly document
            swComponent = (Component2)swAssemblyDoc.**AddComponent5**(strCompModelname, (int)swAddComponentConfigOptions\_e.swAddComponentConfigOptions\_CurrentSelectedConfig, "", false, "", -1, -1, -1);

            // Make the component virtual
            stat = swComponent.**MakeVirtual2**(true);

            // Get the name of the component for the mate
            strCompName = swComponent.**Name2**;

            // Create the name of the mate and the names of the planes to use for the mate
            MateName = "top\_coinc\_" + strCompName;
            FirstSelection = "Top@" + strCompName + "@" + AssemblyName;
            SecondSelection = "Front@" + AssemblyName;

            swModel.**ClearSelection2**(true);
            swDocExt = (ModelDocExtension)swModel.**Extension**;

            // Select the planes for the mate
            boolstat = swDocExt.**SelectByID2**(FirstSelection, "PLANE", 0, 0, 0, true, 1, null, (int)swSelectOption\_e.swSelectOptionDefault);
            boolstat = swDocExt.**SelectByID2**(SecondSelection, "PLANE", 0, 0, 0, true, 1, null, (int)swSelectOption\_e.swSelectOptionDefault);

            // Add the mate
            matefeature = (Feature)swAssemblyDoc.**AddMate5**((int)swMateType\_e.swMateCOINCIDENT, (int)swMateAlign\_e.swMateAlignALIGNED, false, 0, 0, 0, 0, 0, 0, 0, 0, false, false,
0, out mateError);
            matefeature.**Name** = MateName;
            Debug.Print("Mate
added: " + matefeature.**Name**);

            swModel.**ViewZoomtofit2**();

        }

        public void AttachEventHandlers()
        {
            AttachSWEvents();
        }

        public void AttachSWEvents()
        {
            swAssemblyDoc.**AddItemNotify** += this.swAssemblyDoc\_AddItemNotify;
            swAssemblyDoc.**RenameItemNotify** += this.swAssemblyDoc\_RenameItemNotify;
        }

        private int swAssemblyDoc\_AddItemNotify(int EntityType, string itemName)
        {
            Debug.Print("Component added: " + itemName);
            return 1;
        }

        private int swAssemblyDoc\_RenameItemNotify(int EntityType, string oldName, string NewName)
        {
            Debug.Print("Virtual component name: " + NewName);
            return 1;
        }

        public SldWorks swApp;

    }
}