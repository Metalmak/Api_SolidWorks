<!-- source: sldworksapi/Hide_the_FeatureManager_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Hide the FeatureManager Design Tree Example (C#)

This example shows how to hide the FeatureManager design tree.

//--------------------------------------------
// Preconditions: Open a model document.
//
// Postconditions:
// 1. Hides the FeatureManager design tree.
// 2. Examine SOLIDWORKS.
//--------------------------------------------
using
SolidWorks.Interop.sldworks;
using
SolidWorks.Interop.swconst;
using
System;
namespace
HideFeatureManager\_CSharp.csproj
{
    partial
class
SolidWorksMacro
    {

        void
Main()
        {

            ModelDoc2
swModel;
            ModelDocExtension
swModDocExt;
            bool
bRet;

            swModel = (ModelDoc2)swApp.**ActiveDoc**;
            swModDocExt = swModel.**Extension**;
            bRet = swModDocExt.**HideFeatureManager**(true);
        }

        public
SldWorks
swApp;

    }
}