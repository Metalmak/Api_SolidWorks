<!-- source: sldworksapi/Add_ActiveX_Tabs_to_FeatureManager_Design_Tree_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Add ActiveX Tabs to FeatureManager Design Tree  Example (C#)

This example shows how to add tabs to a split FeatureManager design tree
using an on-disk bitmap file for the tabs' icons.

//----------------------------------------------------------
// Preconditions:
// 1. In the IDE,
reference your ActiveX control file
//    (click **Project > Add Reference > Browse** and
browse
//    to the folder where the ActiveX control resides and
click
//    the ActiveX control file **> OK**).
// 2. Verify that the specified part document and bitmap exist.
// 3. Replace *activex\_control\_component\_declaration* and
//    *activex\_control\_CLSID\_or\_ProgID* with your
ActiveX control's
//    information.
//
// Postconditions:
// 1. Opens the part document and splits the FeatureManager
//    design tree.
// 2. Adds a new tab to each FeatureManager design tree.
// 3. Activates the new tab on the top FeatureManager
//    design tree.
//
// NOTE: Because the part document is used elsewhere,
// do not save changes.
//----------------------------------------------------------
using
SolidWorks.Interop.sldworks;
using
SolidWorks.Interop.swconst;

namespace
AddTabsFeatureManagerDesignTreeCSharp.csproj
{
    partial
class
SolidWorksMacro
    {
        public
void Main()
        {
            const
string
iconSmall = "C:\\Program
Files\\SOLIDWORKS Corp\\SOLIDWORKS\\data\\user macro icons\\button.bmp";

            ModelDoc2 swModel = default(ModelDoc2);
            ModelViewManager swModViewMgr =
default(ModelViewManager);
            FeatMgrView swFeatMgrTabTop =
default(FeatMgrView);
            FeatMgrView swFeatMgrTabBtm =
default(FeatMgrView);
            *activex\_control\_component\_declaration* ctrlTop =
default(*activex\_control\_component\_declaration*);
            *activex\_control\_component\_declaration* ctrlBtm =
default(*activex\_control\_component\_declaration*);
            string
fileName = null;
            int
errors = 0;
            int
warnings = 0;
            int
activePane = 0;

            fileName = "C:\\Users\\Public\\Documents\\SOLIDWORKS\SOLIDWORKS
2018\\samples\\tutorial\\fillets\\knob.sldprt";
            swModel = (ModelDoc2)swApp.**OpenDoc6**(fileName, (int)swDocumentTypes\_e.swDocPART,
(int)swOpenDocOptions\_e.swOpenDocOptions\_Silent,
"",
ref errors,
ref
warnings);

            swModViewMgr = (ModelViewManager)swModel.**ModelViewManager**;

            // Split the FeatureManager
design tree;
            //
the original is displayed below the copy
            swModel.**FeatureManagerSplitterPosition**
= 0.5;

            // New tab on copy of
FeatureManager design tree
            swFeatMgrTabBtm =
(FeatMgrView)swModViewMgr.**CreateFeatureMgrControl2**(iconSmall,
"*activex\_control\_CLSID\_or\_ProgID*",
"",
"Bottom tab ToolTip",
(int)swFeatMgrPane\_e.swFeatMgrPaneBottom);
            ctrlBtm = (*activex\_control\_component\_declaration*)swFeatMgrTabBtm.**GetControl**();

            //
New tab on original of FeatureManager design tree
            swFeatMgrTabTop =
(FeatMgrView)swModViewMgr.**CreateFeatureMgrControl2**(iconSmall,
"*activex\_control\_CLSID\_or\_ProgID*",
"",
"Top tab ToolTip",
(int)swFeatMgrPane\_e.swFeatMgrPaneTop);
            ctrlTop = (*activex\_control\_component\_declaration*)swFeatMgrTabTop.**GetControl**();
            activePane =
swFeatMgrTabTop.**ActivateView**();
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