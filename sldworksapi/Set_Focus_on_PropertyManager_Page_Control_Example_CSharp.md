<!-- source: sldworksapi/Set_Focus_on_PropertyManager_Page_Control_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Set Focus on PropertyManager Page Control Example (C#)

This example shows how to set focus on a PropertyManager
page control.

```
//----------------------------------------------------------------------------
// Preconditions:
// 1. Open a model document.
// 2. Copy Main to the main module.
// 3. Click Project > Add Class > Add and copy Class1 to Class1.cs.
// 4. Click Project > Add Reference > browse to install_dir\api\redist,
//    select SolidWorks.Interop.swpublished.dll < OK.
// 5. Open the Immediate window.
//
// Postconditions:
// 1. Creates and displays a PropertyManager page.
// 2. Select the check box to set focus on Text box.
// 3. Examine the Immediate window.
// 4. Clear the check box to remove focus from Text box.
// 5. Examine the Immediate window.
// 6. Click OK to close the PropertyManager page.
//---------------------------------------------------------------------------
//Main
using SolidWorks.Interop.sldworks;
using SolidWorks.Interop.swconst;
using System.Runtime.InteropServices;
using System;

namespace Macro1CSharp.csproj
{
    partial class SolidWorksMacro
    {
        public ModelDoc2 Part;
        public Class1 pm;

        public void Main()
        {
            swApp.SetUserPreferenceToggle((int)swUserPreferenceToggle_e.swStopDebuggingVstaOnExit, false);
            Part = (ModelDoc2)swApp.ActiveDoc;

            //Create a new instance of the PropertyManager class
            pm = new Class1(swApp);
            pm.Show();
        }

        /// <summary>
        ///  The SldWorks swApp variable is pre-assigned for you.
        /// </summary>
        public SldWorks swApp;
    }
}
```

[Back to top](#Top)

//Class1
using SolidWorks.Interop.sldworks;
using SolidWorks.Interop.swconst;
using SolidWorks.Interop.swpublished;
using System;
using System.Runtime.InteropServices;
using System.Diagnostics;

namespace Macro1CSharp.csproj
{

    [ComVisibleAttribute(true)]
    public class Class1 : PropertyManagerPage2Handler9
    {
        //General objects required for the PropertyManager page
        PropertyManagerPage2 pm\_Page;
        PropertyManagerPageGroup pm\_Groupbox;
        PropertyManagerPageCheckbox pm\_Checkbox;
        PropertyManagerPageTextbox pm\_Textbox;

        //Each object in the page needs a unique ID
        const int groupboxID = 1;
        const int checkboxID = 2;
        const int textboxID = 3;

        public void Show()
        {
            pm\_Page.**Show2**(0);
        }

        //The following runs when a new instance
        //of the class is created
        public Class1(SldWorks swApp)
        {
            string pageTitle = null;
            string caption = null;
            long options = 0;
            int errors = 0;
            int control = 0;
            int alignment = 0;

            //Set the variables for the page
            pageTitle = "Test focus methods";
            options = (int)swPropertyManagerButtonTypes\_e.swPropertyManager\_OkayButton + (int)swPropertyManagerButtonTypes\_e.swPropertyManager\_CancelButton + (int)swPropertyManagerPageOptions\_e.swPropertyManagerOptions\_LockedPage + (int)swPropertyManagerPageOptions\_e.swPropertyManagerOptions\_PushpinButton;

            //Create the PropertyManager page
            pm\_Page = (PropertyManagerPage2)swApp.**CreatePropertyManagerPage**(pageTitle, (int)options, this, ref errors);
            //Make sure that the page was created properly
            if (errors == (int)swPropertyManagerPageStatus\_e.swPropertyManagerPage\_Okay)
            {
                //Begin adding the controls to the page
                //Create group box
                caption = "Group box";
                options = (int)swAddGroupBoxOptions\_e.swGroupBoxOptions\_Visible + (int)swAddGroupBoxOptions\_e.swGroupBoxOptions\_Expanded;
                pm\_Groupbox = (PropertyManagerPageGroup)pm\_Page.**AddGroupBox**(groupboxID, caption, (int)options);

                // Create check box
                control = (int)swPropertyManagerPageControlType\_e.swControlType\_Checkbox;
                caption = "Focus on text box";
                alignment = (int)swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_LeftEdge;
                options = (int)swAddControlOptions\_e.swControlOptions\_Visible + (int)swAddControlOptions\_e.swControlOptions\_Enabled;
                pm\_Checkbox = (PropertyManagerPageCheckbox)pm\_Groupbox.**AddControl**(checkboxID, (short)control, caption, (short)alignment, (int)options, "");
                Debug.Print("Upon opening the PropertyManager page:");
                Debug.Print("  State of check box: (0 = Unchecked, 1 = Checked, 2 = Indeterminate): " + pm\_Checkbox.**State**);
                pm\_Checkbox.**Checked** = false;

                // Create text box
                control = (int)swPropertyManagerPageControlType\_e.swControlType\_Textbox;
                caption = "Text box";
                pm\_Textbox = (PropertyManagerPageTextbox)pm\_Groupbox.**AddControl**(textboxID, (short)control, caption, (short)alignment, (int)options, "");
            }
            else
            {
                //If the page is not created
                System.Windows.Forms.MessageBox.Show("An error occurred while attempting to create the PropertyManager page");
            }
        }

        #region IPropertyManagerPage2Handler9 Members

        void IPropertyManagerPage2Handler9.**AfterActivation**()
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**AfterClose**()
        {
            throw new Exception("The method or operation is not implemented.");
        }

        int IPropertyManagerPage2Handler9.**OnActiveXControlCreated**(int Id, bool Status)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnButtonPress**(int Id)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnCheckboxCheck**(int Id, bool Checked)
        {
            Debug.Print("Upon clicking the check box on the PropertyManager page:");
            Debug.Print("  State of check box: (0 = Unchecked, 1 = Checked, 2 = Indeterminate): " + pm\_Checkbox.**State**);
            // Set focus on the text box when check box is selected
            if (Checked)
            {
                pm\_Page.**SetFocus**(textboxID);
                Debug.Print("Focus on Text box.");
            }
            else
            {
                Debug.Print("Focus off Text box.");
            }
        }

        void IPropertyManagerPage2Handler9.**OnClose**(int Reason)
        {
            if (Reason == (int)swPropertyManagerPageCloseReasons\_e.swPropertyManagerPageClose\_Cancel)
            {
                //Do something when the cancel button is clicked
            }
            else if (Reason == (int)swPropertyManagerPageCloseReasons\_e.swPropertyManagerPageClose\_Okay)
            {
                //Do something else when the OK button is clicked
            }
        }

        void IPropertyManagerPage2Handler9.**OnComboboxEditChanged**(int Id, string Text)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnComboboxSelectionChanged**(int Id, int Item)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnGainedFocus**(int Id)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnGroupCheck**(int Id, bool Checked)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnGroupExpand**(int Id, bool Expanded)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        bool IPropertyManagerPage2Handler9.**OnHelp**()
        {
            throw new Exception("The method or operation is not implemented.");
        }

        bool IPropertyManagerPage2Handler9.**OnKeystroke**(int Wparam, int Message, int Lparam, int Id)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnListboxSelectionChanged**(int Id, int Item)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnLostFocus**(int Id)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        bool IPropertyManagerPage2Handler9.**OnNextPage**()
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnNumberboxChanged**(int Id, double Value)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnOptionCheck**(int Id)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnPopupMenuItem**(int Id)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnPopupMenuItemUpdate**(int Id, ref int retval)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        bool IPropertyManagerPage2Handler9.**OnPreview**()
        {
            throw new Exception("The method or operation is not implemented.");
        }

        bool IPropertyManagerPage2Handler9.**OnPreviousPage**()
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnRedo**()
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnSelectionboxCalloutCreated**(int Id)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnSelectionboxCalloutDestroyed**(int Id)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnSelectionboxFocusChanged**(int Id)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnSelectionboxListChanged**(int Id, int Count)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnSliderPositionChanged**(int Id, double Value)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnSliderTrackingCompleted**(int Id, double Value)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        bool IPropertyManagerPage2Handler9.**OnSubmitSelection**(int Id, object Selection, int SelType, ref string ItemText)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        bool IPropertyManagerPage2Handler9.**OnTabClicked**(int Id)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnTextboxChanged**(int Id, string Text)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnUndo**()
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnWhatsNew**()
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnListboxRMBUp**(int Id, int PosX, int PosY)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        int IPropertyManagerPage2Handler9.**OnWindowFromHandleControlCreated**(int Id, bool Status)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        void IPropertyManagerPage2Handler9.**OnNumberBoxTrackingCompleted**(int Id, double Value)
        {
            throw new Exception("The method or operation is not implemented.");
        }

        #endregion

    }

}

[Back to top](#Top)