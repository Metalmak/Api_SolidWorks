<!-- source: sldworksapi/Split_FeatureManager_Design_Tree_and_Position_Splitter_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Split FeatureManager Design Tree and Position Splitter Example (C#)

This example shows how:

* to split a FeatureManager design tree.
* add a tab to one of the FeatureManager design trees.
* change the location of the split panel bar (splitter).

//----------------------------------------------------------
// Preconditions:
// 1. In the IDE, reference
your ActiveX control file
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
//
design tree; the splitter is
below the FeatureManager
//
design tree to which the
tab was added. Drag the splitter
//    to verify.
// 2. Close the part document.
// 3. Set test to 1.
// 4. Rerun the macro.
// 5. Opens the part document and splits the FeatureManager
//
design tree; the splitter is
above the FeatureManager
//
design tree to which the
tab was added. Drag the
//    splitter to verify.
//
// NOTE: Because the part document is used elsewhere,
// do not save changes.
//----------------------------------------------------------
using
SolidWorks.Interop.sldworks;
using
SolidWorks.Interop.swconst;
using
System;

namespace
FeatureManagerSplitterPositionModelDoc2CSharp.csproj
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
            int
test = 0;

            fileName = "C:\\Users\\Public\\Documents\\SOLIDWORKS\SOLIDWORKS
2018\\samples\\tutorial\\fillets\\knob.sldprt";
            swModel = (ModelDoc2)swApp.**OpenDoc6**(fileName, (int)swDocumentTypes\_e.swDocPART,
(int)swOpenDocOptions\_e.swOpenDocOptions\_Silent,
"",
ref errors,
ref
warnings);
            swModViewMgr = (ModelViewManager)swModel.**ModelViewManager**;

            if
(test == 0)
            {
                // FeatureManager design
tree is split, and the splitter is
                //
below the FeatureManager design tree to which the
                //
tab was added
                swFeatMgrTabTop =
(FeatMgrView)swModViewMgr.**CreateFeatureMgrControl2**(iconSmall,
"*activex\_control\_CLSID\_or\_ProgID*",
"",
"Top tab ToolTip",
(int)swFeatMgrPane\_e.swFeatMgrPaneTop);
                ctrlTop = (*activex\_control\_component\_declaration*)swFeatMgrTabTop.**GetControl**();
                swModel.**FeatureManagerSplitterPosition** = 0.0;
                activePane = swFeatMgrTabTop.**ActivateView**();
            }
            else
            {
                // FeatureManager design
tree is split, and the splitter is
                //
above the FeatureManager design tree to which the
                //
tab was added
                swFeatMgrTabBtm =
(FeatMgrView)swModViewMgr.**CreateFeatureMgrControl2**(iconSmall,
"*activex\_control\_CLSID\_or\_ProgID*",
"",
"Bottom tab ToolTip",
(int)swFeatMgrPane\_e.swFeatMgrPaneBottom);
                ctrlBtm = (*activex\_control\_component\_declaration*)swFeatMgrTabBtm.**GetControl**();
                swModel.**FeatureManagerSplitterPosition** = 1.0;
                activePane = swFeatMgrTabBtm.**ActivateView**();
            }
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