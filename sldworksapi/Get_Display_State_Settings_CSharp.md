<!-- source: sldworksapi/Get_Display_State_Settings_CSharp.htm -->

# SOLIDWORKS API Help

# Get Display State Settings Example (C#)

This example shows how to get display modes, transparency states, and
visibility states of components.

//------------------------------------------------------------------------------
// Preconditions: Open an assembly that contains a minimum of three
top-level
// components and two display states, "DS\_1" and "DS\_2".
//
// Postconditions: Inspect the Immediate Window for the display modes,
// transparency states, and visibility states of all three components
// in both DS\_1 and DS\_2.
//-----------------------------------------------------------------------------
using
SolidWorks.Interop.sldworks;
using
SolidWorks.Interop.swconst;
using
System;
using
System.Diagnostics;
namespace
GetDisplayMode.csproj
{
    public
partial
class
SolidWorksMacro
    {
        ModelDoc2
swDoc = null;
        ModelDocExtension
swExt = null;
        DisplayStateSetting
swDSS = null;
        object
varStatus;
        object
varTStatus;
        object
varVStatus;
        Array
statusArray;
        Array
statusTArray;
        Array
statusVArray;
        const
int
maxEntMode = 3;

        public
void Main()
        {
            swDoc = (ModelDoc2)(swApp.ActiveDoc);
            swExt = swDoc.Extension;
            int
docType = swDoc.GetType();
            if
(docType == (int)swDocumentTypes\_e.swDocASSEMBLY)
            {
                CreateDisplayStateSetting();

                varStatus = swExt.**get\_DisplayMode**(swDSS);
                statusArray = (Array)varStatus;

                varTStatus = swExt.**get\_Transparency**(swDSS);
                statusTArray = (Array)varTStatus;

                varVStatus = swExt.**get\_Visibility**(swDSS);
                statusVArray = (Array)varVStatus;

                WriteOutput();
            }
        }

        public
void
CreateDisplayStateSetting()
        {
            swDSS = swExt.**GetDisplayStateSetting**((int)swDisplayStateOpts\_e.swThisDisplayState);
            swDSS.Option = (int)swDisplayStateOpts\_e.swSpecifyDisplayState;

            string[]
specDSNames = new
string[2];
            specDSNames[0] = "DS\_1";
            specDSNames[1] = "DS\_2";
            object
varSpecDSNames = specDSNames;
            swDSS.**Names** = varSpecDSNames;

            AssemblyDoc
swADoc;
            swADoc = (AssemblyDoc)swDoc;
            int
compCnt = swADoc.GetComponentCount(true);
            Component2[]
listComp = new
Component2[maxEntMode];
            if
(compCnt >= maxEntMode)
            {
                object[]
varComp = (object[])(swADoc.GetComponents(true));
                listComp[0] = (Component2)varComp[0];
                listComp[1] = (Component2)varComp[1];
                listComp[2] = (Component2)varComp[2];
                swDSS.**Entities** = listComp;
            }

        }

        public
void
WriteOutput()
        {
            int
entCount = swDSS.**GetEntityCount**();
            object[]
listComp = (object[])swDSS.**Entities**;
            int
allCtr = 0;
            for
(int entctr
= 0; entctr < entCount; ++entctr)
            {
                Component2
swComp = (Component2)listComp[entctr];
                Debug.Print(swComp.Name2);
                int
dsNameCount = swDSS.**GetNameCount**();
                object[]
dsNames = (object[])swDSS.**Names**;

                for
(int
namectr = 0; namectr < dsNameCount; ++namectr)
                {
                    Debug.Print("
" + (string)dsNames[namectr]);
                    int
status = (int)statusArray.GetValue(allCtr);
                    int
statusT = (int)statusTArray.GetValue(allCtr);
                    int
statusV = (int)statusVArray.GetValue(allCtr);
                    WriteMode(status);
                    WriteTransparency(statusT);
                    WriteVisibility(statusV);
                    ++allCtr;
                }
            }
        }
        public
void
WriteMode(int
status)
        {
            switch
(status)
            {
                case
(int)swDisplayMode\_e.swDisplayModeDEFAULT:
                    Debug.Print("
swDisplayModeDEFAULT");
                    break;
                case
(int)swDisplayMode\_e.swHIDDEN:
                    Debug.Print("
swHIDDEN");
                    break;
                case
(int)swDisplayMode\_e.swHIDDEN\_GREYED:
                    Debug.Print("
swHIDDEN\_GREYED");
                    break;
                case
(int)swDisplayMode\_e.swSHADED:
                    Debug.Print("
swSHADED");
                    break;
                case
(int)swDisplayMode\_e.swSHADED\_EDGES:
                    Debug.Print("
swSHADED\_EDGES");
                    break;
                case
(int)swDisplayMode\_e.swWIREFRAME:
                    Debug.Print("
swWIREFRAME");
                    break;
                case
(int)swDisplayMode\_e.swDisplayModeUNKNOWN:
                    Debug.Print("
Error:swDisplayModeUNKNOWN");
                    break;

Case CInt(swDisplayMode\_e.swFACETED\_WIREFRAME)
                    Debug.Print
("
swFACETED\_WIREFRAME")
                    break;

    Case CInt(swDisplayMode\_e.swFACETED\_HIDDEN\_GREYED)
                    Debug.Print
("
swFACETED\_HIDDEN\_GREYED")
                    break;

    Case CInt(swDisplayMode\_e.swFACETED\_HIDDEN)
                    Debug.Print
("
swFACETED\_HIDDEN")
                    break;

            }
        }
        public
void
WriteTransparency(int
status)
        {
            switch
(status)
            {
                case
(int)swTransparencyState\_e.swTransparencyStateTransparent:
                    Debug.Print("
swTransparencyStateTransparent");
                    break;
                case
(int)swTransparencyState\_e.swTransparencyStateNonTransparent:
                    Debug.Print("
swTransparencyStateNonTransparent");
                    break;
                case
(int)swTransparencyState\_e.swTransparencyStateUnknown:
                    Debug.Print("
ERROR : swTransparencyStateUnknown");
                    break;
            }
        }
        public
void
WriteVisibility(int
status)
        {
            switch
(status)
            {
                case
(int)swVisibilityState\_e.swVisibilityStateHide:
                    Debug.Print("
swVisibilityStateHide");
                    break;
                case
(int)swVisibilityState\_e.swVisibilityStateShown:
                    Debug.Print("
swVisibilityStateShown");
                    break;
                case
(int)swVisibilityState\_e.swVisibilityStateUnknown:
                    Debug.Print("
ERROR : swVisibilityStateUnknown");
                    break;
            }
        }

        public
SldWorks
swApp;
    }
}