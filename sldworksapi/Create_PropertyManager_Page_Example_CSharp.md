<!-- source: sldworksapi/Create_PropertyManager_Page_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Create PropertyManager Page Example (C#)

This example shows how to create a PropertyManager
page that contains these controls:

* ActiveX
* Bitmap
* Bitmap buttons
* Button
* Combo box
* Group box
* Label
* List box
* Number box
* Radio button
* Selection box
* Slider
* Tab

This
example also shows how to handle focus events for these controls.

NOTE: If the model is an assembly
that contains multiple components and you want to allow the user to
select edges, faces, or vertices, then you must specify swSelectType\_e.swSelCOMPSDONTOVERRIDE
for parameter SelType of IPropertyManagerPageSelectionbox::SetSelectionFilters.
Otherwise, if the user attempts to select an edge, face, or vertex, then the
entire component might get selected and not the edge, face, or vertex. This
example demonstrates how to specify SelType.

//-------------------------------------------------------------------------
// Preconditions:

//  1  Create
a C# macro named **CreatePropertyManagerPageExample\_CSharp.**
//  2. Copy
and paste
[Main](#Modules) into **SolidWorksMacro.cs**.
//  3. Add a class named **clsPropMgr** and copy and paste
[clsPropMgr](#Class)
into that class.
//  4. Click **Project >** Add Reference,
browse to i*nstall\_dir***\api\redist\**, select

//     SolidWorks.Interop.swpublished.dll
> OK.
//  5. Verify that the specified assembly document
exists.
//  6. Modify *ClassID* and *LicenseKey*
parameters in
//     IPropertyManagerPageActiveX::SetClass to add your ActiveX
control
//     to the PropertyManager page.
//  7. Replace the ImageList and
ImageListMasks array elements
//     with the pathnames of your image files.
//  8. Open an Immediate window.
//
// Postconditions:
//  1. Opens the specified assembly.
//  2. Creates a PropertyManager page.
//  3. Creates the specified controls.
//  4. Examine the Immediate Window as you use the specified
//     controls. Note the size of the button at the bottom

//     of the PropertyManager page.
//  5. Click **OK** to close the PropertyManager page.
//  6. Exit SOLIDWORKS.
//  7. Change the size of the text and other items on your computer.
//     For example, in Windows 7:
//     a. Click **Start > Control Panel > Appearance and**
//        **Personalization > Display**.
//     b. Select a different size.
//     c. Click **Apply**.
//     d. Click **Log off now**.
//     e. Log back in.
//  8. Start SOLIDWORKS.
//  9. Run this macro again and note the size of the button at
//     the bottom of the PropertyManager page.
// 10. Click **OK** to close the PropertyManager page.
//
// **NOTES**:
// \*
After running this
macro, select
//   Tools
> Options > System Options > Stop VSTA debugger

//   on
macro exit.
// \*
Because
the assembly document is used elsewhere,
//   do not save changes.
//---------------------------------------------------------------------------

//Main

using SolidWorks.Interop.sldworks;
using SolidWorks.Interop.swconst;
using System;

namespace CreatePropertyManagerPageExample\_CSharp.csproj

{

    partial
class SolidWorksMacro

    {

        public
ModelDoc2 Part;
        public
clsPropMgr pm;

        public
void Main()

        {

            int
openDocErrors = 0;
            int
openDocWarnings = 0;

            swApp.SetUserPreferenceToggle((int)swUserPreferenceToggle\_e.swStopDebuggingVstaOnExit,
false);

            Part
= swApp.OpenDoc6("C:\\Users\\Public\\Documents\\SOLIDWORKS\\SOLIDWORKS
2018\\samples\\tutorial\\advdrawings\\bladed
shaft.sldasm", (int)swDocumentTypes\_e.swDocASSEMBLY, (int)swOpenDocOptions\_e.swOpenDocOptions\_Silent,
"", ref openDocErrors, ref openDocWarnings);

            //Create
a new instance of the PropertyManager class
            pm
= new clsPropMgr(swApp);
            pm.Show();

        }

        public
SldWorks swApp;

    }

}

[Back to top](#Top)

//clsPropMgr

using SolidWorks.Interop.sldworks;
using SolidWorks.Interop.swconst;
using SolidWorks.Interop.swpublished;
using System;
using System.Runtime.InteropServices;
using System.Diagnostics;

namespace CreatePropertyManagerPageExample\_CSharp.csproj

{

    [ComVisibleAttribute(true)]
    public
class clsPropMgr : PropertyManagerPage2Handler9

    {

//Control objects required for the PropertyManager page
        PropertyManagerPage2 pm\_Page;
        PropertyManagerPageGroup pm\_Group;
        PropertyManagerPageSelectionbox pm\_Selection;
        PropertyManagerPageSelectionbox pm\_Selection2;
        PropertyManagerPageLabel pm\_Label;
        PropertyManagerPageCombobox pm\_Combo;
        PropertyManagerPageListbox pm\_List;
        PropertyManagerPageNumberbox pm\_Number;
        PropertyManagerPageOption pm\_Radio;
        PropertyManagerPageSlider pm\_Slider;
        PropertyManagerPageTab pm\_Tab;
        PropertyManagerPageButton pm\_Button;
        PropertyManagerPageBitmapButton pm\_BMPButton;
        PropertyManagerPageBitmapButton pm\_BMPButton2;
        PropertyManagerPageBitmap pm\_Bitmap;
        PropertyManagerPageActiveX pm\_ActiveX;

        //Each control in the page needs a unique ID
        const int GroupID = 1;
        const int LabelID = 2;
        const int SelectionID = 3;
        const int ComboID = 4;
        const int ListID = 5;
        const int Selection2ID = 6;
        const int NumberID = 7;
        const int RadioID = 8;
        const int SliderID = 9;
        const int TabID = 10;
        const int ButtonID = 11;
        const int BMPButtonID = 12;
        const int BMPButtonID2 = 13;
        const int BitmapID = 14;
        const int ActiveXID = 15;

        public
void Show()

        {

            pm\_Page.Show2(0);

        }

        //The
following runs when a new instance
        //of
the class is created
        public
clsPropMgr(SldWorks swApp)
        {

            string
PageTitle = null;
            string
caption = null;
            string
tip = null;
            int
options = 0;
            int
longerrors = 0;
            int
controlType = 0;
            int
alignment = 0;
            string[]
listItems = new string[4];

            //Set
the variables for the page
            PageTitle
= "Comps";
            options
= (int)swPropertyManagerButtonTypes\_e.swPropertyManager\_OkayButton + (int)swPropertyManagerButtonTypes\_e.swPropertyManager\_CancelButton
+ (int)swPropertyManagerPageOptions\_e.swPropertyManagerOptions\_LockedPage
+ (int)swPropertyManagerPageOptions\_e.swPropertyManagerOptions\_PushpinButton;

            //Create
the PropertyManager page
            pm\_Page
= (PropertyManagerPage2)swApp.CreatePropertyManagerPage(PageTitle,
(int)options, this, ref longerrors);

            //Make
sure that the page was created properly
            if
(longerrors == (int)swPropertyManagerPageStatus\_e.swPropertyManagerPage\_Okay)

            {

                //Add the controls to the page

//Add a tab

         pm\_Tab = pm\_Page.**AddTab**(TabID, "Application", "", 0);

                 //Add a group box to the tab
                 caption = "Controls";
                 options = (int)swAddGroupBoxOptions\_e.swGroupBoxOptions\_Visible + (int)swAddGroupBoxOptions\_e.swGroupBoxOptions\_Expanded;
                 pm\_Group = (PropertyManagerPageGroup)pm\_Tab.**AddGroupBox**(GroupID, caption, options);

 //Add two selection boxes

 controlType
= (int)swPropertyManagerPageControlType\_e.swControlType\_Selectionbox;
 caption
= "";

                alignment
= (int)swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_Indent;
                options
= (int)swAddControlOptions\_e.swControlOptions\_Visible + (int)swAddControlOptions\_e.swControlOptions\_Enabled;
                tip
= "Select an edge, face, vertex, solid body, or a component";
                pm\_Selection
= (PropertyManagerPageSelectionbox)pm\_Group.AddControl2(SelectionID,
(short)controlType, caption, (short)alignment, (int)options, tip);
                pm\_Selection2
= (PropertyManagerPageSelectionbox)pm\_Group.AddControl2(Selection2ID,
(short)controlType, caption, (short)alignment, (int)options, tip);

                swSelectType\_e[]
filters = new swSelectType\_e[7];
                filters[0]
= swSelectType\_e.swSelEDGES;
                filters[1]
= swSelectType\_e.swSelREFEDGES;
                filters[2]
= swSelectType\_e.swSelFACES;
                filters[3]
= swSelectType\_e.swSelVERTICES;
                filters[4]
= swSelectType\_e.swSelSOLIDBODIES;
                filters[5]
= swSelectType\_e.swSelCOMPONENTS;
                filters[6]
= swSelectType\_e.swSelCOMPSDONTOVERRIDE;

                object
filterObj = null;
                filterObj
= filters;

                pm\_Selection.SingleEntityOnly = false;
                pm\_Selection.AllowMultipleSelectOfSameEntity = true;
                pm\_Selection.Height = 50;
                pm\_Selection.SetSelectionFilters(filterObj);

                pm\_Selection2.SingleEntityOnly = false;
                pm\_Selection2.AllowMultipleSelectOfSameEntity = true;
                pm\_Selection2.Height = 50;
                pm\_Selection2.SetSelectionFilters(filterObj);

                //Add a combo box

                controlType
= (int)swPropertyManagerPageControlType\_e.swControlType\_Combobox;
                caption
= "";
                alignment
= (int)swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_Indent;
                options
= (int)swAddControlOptions\_e.swControlOptions\_Visible + (int)swAddControlOptions\_e.swControlOptions\_Enabled;
                tip
= "Select a value";
                pm\_Combo
= (PropertyManagerPageCombobox)pm\_Group.AddControl2(ComboID,
(short)controlType, caption, (short)alignment, (int)options, tip);
                if
((pm\_Combo != null))
                {
                    pm\_Combo.Height = 50;
                    listItems[0]
= "Value 1";
                    listItems[1]
= "Value 2";
                    listItems[2]
= "Value 3";
                    listItems[3]
= "Value 4";
                    pm\_Combo.AddItems(listItems);
                    pm\_Combo.CurrentSelection = 0;
                }

                //Add a list box

                controlType
= (int)swPropertyManagerPageControlType\_e.swControlType\_Listbox;
                caption
= "";
                alignment
= (int)swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_Indent;
                options
= (int)swAddControlOptions\_e.swControlOptions\_Visible + (int)swAddControlOptions\_e.swControlOptions\_Enabled;
                tip
= "Multi-select values in the list box";
                pm\_List
= (PropertyManagerPageListbox)pm\_Group.AddControl2(ListID,
(short)controlType, caption, (short)alignment, (int)options, tip);

                if
((pm\_List != null))
                {
                    pm\_List.Style = (int)swPropMgrPageListBoxStyle\_e.swPropMgrPageListBoxStyle\_MultipleItemSelect;
                    pm\_List.Height = 50;
                    listItems[0]
= "Value 1";
                    listItems[1]
= "Value 2";
                    listItems[2]
= "Value 3";
                    listItems[3]
= "Value 4";
                    pm\_List.AddItems(listItems);
                    pm\_List.SetSelectedItem(1, true);
                }

//Add a label
        pm\_Label = (PropertyManagerPageLabel)pm\_Group.**AddControl2**(LabelID, (int)swPropertyManagerPageControlType\_e.swControlType\_Label, "Label", (int)swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_LeftEdge, options, "");

            //Add a slider
            pm\_Slider = (PropertyManagerPageSlider)pm\_Group.**AddControl2**(SliderID, (int)swPropertyManagerPageControlType\_e.swControlType\_Slider, "Slider", (int)swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_LeftEdge, options, "Slide");

            //Add a radio button
            pm\_Radio = (PropertyManagerPageOption)pm\_Group.**AddControl2**(RadioID, (int)swPropertyManagerPageControlType\_e.swControlType\_Option, "Radio button", (int)swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_LeftEdge, options, "Select");

            //Add a number box
            pm\_Number = (PropertyManagerPageNumberbox)pm\_Group.**AddControl2**(NumberID, (int)swPropertyManagerPageControlType\_e.swControlType\_Numberbox, "Number box", (int)swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_LeftEdge, options, "Spin");

            //Add a button
            pm\_Button = (PropertyManagerPageButton)pm\_Group.**AddControl2**(ButtonID, (int)swPropertyManagerPageControlType\_e.swControlType\_Button, "Button", (int)swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_LeftEdge, options, "Click");

            //Add a bitmap button
            pm\_BMPButton = (PropertyManagerPageBitmapButton)pm\_Group.**AddControl2**(BMPButtonID, (int)swPropertyManagerPageControlType\_e.swControlType\_BitmapButton, "Bitmap button", (int)swPropertyManagerPageControlLeftAlign\_e.swControlAlign\_LeftEdge, options, "Click");
        pm\_BMPButton.**SetStandardBitmaps**((int)swPropertyManagerPageBitmapButtons\_e.swBitmapButtonImage\_parallel);

```
            //Add another bitmap button that scales with computer's resolution
            pm_BMPButton2 = (PropertyManagerPageBitmapButton)pm_Group.AddControl2(BMPButtonID2, (int)swPropertyManagerPageControlType_e.swControlType_BitmapButton, "Bitmap button", (int)swPropertyManagerPageControlLeftAlign_e.swControlAlign_LeftEdge, options, "Click");
            string[] imageList = new string[3];
            string[] imageListMasks = new string[3];
            imageList[0] = "Pathname_to_nxn_image";
            imageList[1] = "Pathname_to_nnxnn_image";
            imageList[2] = "Pathname_to_nnnxnnn_image";
            imageListMasks[0] = "Pathname_to_mask_nxn_image";
            imageListMasks[1] = "Pathname_to_mask_nnxnn_image";
            imageListMasks[2] = "Pathname_to_mask_nnnxnnn_image";
             pm_BMPButton2.SetBitmapsByName3(imageList, imageListMasks);
```

```
            //Add a bitmap
	    pm_Bitmap = (PropertyManagerPageBitmap)pm_Group.AddControl2(BitmapID, (int)swPropertyManagerPageControlType_e.swControlType_Bitmap, "Bitmap", (int)swPropertyManagerPageControlLeftAlign_e.swControlAlign_LeftEdge, options, "Bitmap");
            pm_Bitmap.SetStandardBitmap((int)swBitmapControlStandardTypes_e.swBitmapControl_Volume);

	    //Add an ActiveX control
	    pm_ActiveX = (PropertyManagerPageActiveX)pm_Group.AddControl2(ActiveXID, (int)swPropertyManagerPageControlType_e.swControlType_ActiveX, "ActiveX", (int)swProper    tyManagerPageControlLeftAlign_e.swControlAlign_LeftEdge, options, "ActiveX control tip");
            pm_ActiveX.SetClass("ClassID", "LicenseKey");
```

            }

            else

            {

                //If
the page is not created
                System.Windows.Forms.MessageBox.Show("An
error occurred while attempting to create the PropertyManager
page.");

            }

        }

#region
IPropertyManagerPage2Handler9
Members

        void
IPropertyManagerPage2Handler9.**AfterActivation**()

        {

        }

        void
IPropertyManagerPage2Handler9.**AfterClose**()

        {

        }

        int
IPropertyManagerPage2Handler9.**OnActiveXControlCreated**(int Id, bool Status)

        {

            Debug.Print("ActiveX
control created");
            return 0;

        }

        void
IPropertyManagerPage2Handler9.**OnButtonPress**(int Id)

        {

Debug.Print("Button clicked");

        }

        void
IPropertyManagerPage2Handler9.**OnCheckboxCheck**(int Id, bool Checked)

        {

        }

        void
IPropertyManagerPage2Handler9.OnClose(int
Reason)

        {

            if
(Reason == (int)swPropertyManagerPageCloseReasons\_e.swPropertyManagerPageClose\_Cancel)

            {

Debug.Print ("Cancel
button clicked");

            }

else
if (Reason == (int)swPropertyManagerPageCloseReasons\_e.swPropertyManagerPageClose\_Okay)

            {

                Debug.Print
("OK button clicked");

            }

        }

        void
IPropertyManagerPage2Handler9.**OnComboboxEditChanged**(int Id, string Text)

        {

        }

        void
IPropertyManagerPage2Handler9.**OnComboboxSelectionChanged**(int Id, int Item)

        {

        }

        void
IPropertyManagerPage2Handler9.OnGainedFocus(int
Id)

        {

            short[]
varArray = null;
            Debug.Print("Control
box " + Id + " gained focus");
            varArray
= (short[])pm\_List.**GetSelectedItems**();
            pm\_Combo.**CurrentSelection**
= varArray[0];

        }

        void
IPropertyManagerPage2Handler9.**OnGroupCheck**(int Id, bool Checked)

        {

        }

        void
IPropertyManagerPage2Handler9.**OnGroupExpand**(int Id, bool Expanded)

        {

        }

        bool
IPropertyManagerPage2Handler9.**OnHelp**()

        {

return false;

        }

        bool
IPropertyManagerPage2Handler9.**OnKeystroke**(int Wparam, int Message, int
Lparam, int Id)

        {

return false;

        }

        void
IPropertyManagerPage2Handler9.**OnListboxSelectionChanged**(int Id, int Item)

        {

        }

        void
IPropertyManagerPage2Handler9.OnLostFocus(int
Id)

        {

            Debug.Print("Control
box " + Id + " lost focus");

        }

        bool
IPropertyManagerPage2Handler9.**OnNextPage**()

        {

return false;

        }

        void
IPropertyManagerPage2Handler9.**OnNumberboxChanged**(int Id, double Value)

        {

Debug.Print("Number box changed");

        }

        void
IPropertyManagerPage2Handler9.**OnOptionCheck**(int Id)

        {

            Debug.Print("Option
selected");

        }

        void
IPropertyManagerPage2Handler9.**OnPopupMenuItem**(int Id)

        {

        }

        void
IPropertyManagerPage2Handler9.**OnPopupMenuItemUpdate**(int Id, ref int retval)

        {

        }

        bool
IPropertyManagerPage2Handler9.**OnPreview**()

        {

return false;

        }

        bool
IPropertyManagerPage2Handler9.**OnPreviousPage**()

        {

return false;

        }

        void
IPropertyManagerPage2Handler9.**OnRedo**()

        {

        }

        void
IPropertyManagerPage2Handler9.**OnSelectionboxCalloutCreated**(int Id)

        {

        }

        void
IPropertyManagerPage2Handler9.**OnSelectionboxCalloutDestroyed**(int Id)

        {

        }

        void
IPropertyManagerPage2Handler9.OnSelectionboxFocusChanged(int
Id)

        {

            Debug.Print("The
focus moved to selection box " + Id);

        }

        void
IPropertyManagerPage2Handler9.OnSelectionboxListChanged(int
Id, int Count)

        {

            pm\_Page.SetCursor((int)swPropertyManagerPageCursors\_e.swPropertyManagerPageCursors\_Advance);
            Debug.Print("The
list in selection box " + Id + " changed");

        }

        void
IPropertyManagerPage2Handler9.**OnSliderPositionChanged**(int Id, double Value)

        {

            Debug.Print("Slider
position changed");

        }

        void
IPropertyManagerPage2Handler9.**OnSliderTrackingCompleted**(int Id, double
Value)

        {

        }

        bool
IPropertyManagerPage2Handler9.OnSubmitSelection(int
Id, object Selection, int SelType, ref string ItemText)

        {

  // This method must return true for selections
to occur
  return
true;

        }

        bool
IPropertyManagerPage2Handler9.**OnTabClicked**(int Id)

        {

return false;

        }

        void
IPropertyManagerPage2Handler9.**OnTextboxChanged**(int Id, string Text)

        {

        }

        void
IPropertyManagerPage2Handler9.**OnUndo**()

        {

        }

        void
IPropertyManagerPage2Handler9.**OnWhatsNew**()

        {

        }

        void
IPropertyManagerPage2Handler9.**OnListboxRMBUp**(int Id, int PosX, int
PosY)
        {

        }

>    int
> IPropertyManagerPage2Handler9.**OnWindowFromHandleControlCreated**(int Id, bool Status)
>    {
>
>         return 0;
>
>    }
>
>    void
> IPropertyManagerPage2Handler9.**OnNumberBoxTrackingCompleted**(int Id, double
> Value)
>    {
>
>    }

        #endregion

    }

}

[Back to top](#Top)