<!-- source: sldworksapi/Create_Local_Circular_Pattern_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Create Local Circular Pattern Example (C#)

This example shows how to create a local circular pattern feature.

//----------------------------------------------------------------
// Preconditions: Verify that the assembly exists.
//
// Postconditions:
// 1. Opens the assembly.
// 2. Selects an edge for the direction axis.
// 3. Selects a subassembly to pattern.
// 4. Creates **LocalCirPattern1**.
// 5. Examine the FeatureManager design tree and graphics area.
//

// NOTE: Because the assembly is used elsewhere, do not
// save changes.

//--------------------------------------------------------
using SolidWorks.Interop.sldworks;
using SolidWorks.Interop.swconst;
using System.Runtime.InteropServices;
using System;
namespace CreateLocalCircularPattern\_CSharp
{

    partial class SolidWorksMacro
    {

        private ModelDoc2 swModel;
        private ModelDocExtension swModelDocExt;
        private FeatureManager swFeatureManager;
        private Feature swFeature;
        private LocalCircularPatternFeatureData swLocalCirPattFD;
        private bool status;
        private int errors = 0;
        private int warnings = 0;
        private string fileName;
        public void Main()
        {

            fileName = "C:\\Users\\Public\\Documents\\SOLIDWORKS\\SOLIDWORKS 2019\\samples\\tutorial\\api\\distance linkage.sldasm";
            swModel = swApp.OpenDoc6(fileName, (int)swDocumentTypes\_e.swDocASSEMBLY, (int)swOpenDocOptions\_e.swOpenDocOptions\_Silent, "", errors, warnings);
            swModelDocExt = swModel.Extension;
            swFeatureManager = swModel.FeatureManager;
            status = swModelDocExt.SelectByID2("", "EDGE", 0.22639417933982, -0.194822643434378, 0.102086175644843, false, 2, null, 0);
            status = swModelDocExt.SelectByID2("mount base-1@distance linkage", "COMPONENT", 0, 0, 0, true, 1, null, 0);
            swLocalCirPattFD = (LocalCircularPatternFeatureData)swFeatureManager.**CreateDefinition**((int)swFeatureNameID\_e.swFmLocalCirPattern);
            swLocalCirPattFD.**TotalInstances** = 3;
            swLocalCirPattFD.**EqualSpacing** = true;
            swFeature = swFeatureManager.**CreateFeature**(swLocalCirPattFD);
            swModel.ClearSelection2(true);

        }

        /// <summary>
        /// The SldWorks swApp variable is pre-assigned for you.
        /// </summary>
        public SldWorks swApp;
    }

}