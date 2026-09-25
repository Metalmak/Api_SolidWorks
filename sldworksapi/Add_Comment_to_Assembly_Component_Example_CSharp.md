<!-- source: sldworksapi/Add_Comment_to_Assembly_Component_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Add Comment to Assembly Component Example (C#)

This example shows how to add a comment to an assembly component.

//----------------------------------------------------------------------------
// Preconditions:
// 1. Open an assembly document.
// 2. Select a component in the FeatureManager design tree.
// 3. Open an Immediate window.
//
// Postconditions: A comment about the selected component is added to the
// document's Comments folder.
//
---------------------------------------------------------------------------
using
SolidWorks.Interop.sldworks;
using
SolidWorks.Interop.swconst;
using
System.Runtime.InteropServices;
using
System;

namespace
AddComment\_C\_.csproj
{
    public
partial
class
SolidWorksMacro
    {

        public
void Main()
        {
            ModelDoc2
swModel;
            SelectionMgr
swSelMgr;
            ModelDocExtension
swModelDocExt;
            Component2
selComp;
            String
selCompName;
            Comment
newComment;

            swModel = (ModelDoc2)swApp.**ActiveDoc**;
            swSelMgr = (SelectionMgr)swModel.**SelectionManager**;
            swModelDocExt = swModel.**Extension**;

            selComp = (Component2)swSelMgr.**GetSelectedObjectsComponent4**(1,
-1);
            selCompName = selComp.**Name2**;

            newComment = swModelDocExt.**AddComment**("This
component's name is " + selCompName);

        }

        public
SldWorks
swApp;
    }
}