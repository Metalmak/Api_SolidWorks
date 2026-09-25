<!-- source: sldworksapi/Create_Multiple_Radius_Fillets_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Create Multiple-Radius Fillets Example (C#)

This example shows how to create multiple-radius fillets.

//--------------------------------------------------------------------------
// Preconditions:
// 1. Open *public\_documents***\samples\tutorial\api\box.sldprt**.
// 2. Select three intersecting edges on the inside of the part.
//
// Postconditions:
// 1. Fillets the three selected edges using three
//    different radii.
// 2. Examine the graphics area and FeatureManager design tree.
//
// Note: Because the model is used elsewhere, do not save changes.
//---------------------------------------------------------------------------
using
SolidWorks.Interop.sldworks;
using
SolidWorks.Interop.swconst;
using
System.Runtime.InteropServices;
using
System;
namespace
FilletFeature\_CSharp.csproj
{
    partial
class
SolidWorksMacro
    {

        ModelDoc2
swModel;
        ModelDocExtension
swModelDocExt;
        FeatureManager
swFeatMgr;
        object
VarRadArray8;
        double[]
radArray8 = new
double[3];

        int
FilletOptions;

        public
void Main()
        {
            swModel = (ModelDoc2)swApp.**ActiveDoc**;
            swModelDocExt = swModel.**Extension**;
            swFeatMgr = swModel.**FeatureManager**;

            //Multiple Radii
            radArray8[0] = 0.01;
            radArray8[1] = 0.015;
            radArray8[2] = 0.02;
            VarRadArray8 = radArray8;

            //Fillet options
            FilletOptions = (int)swFeatureFilletOptions\_e.swFeatureFilletPropagate
+ (int)swFeatureFilletOptions\_e.swFeatureFilletAttachEdges
+ (int)swFeatureFilletOptions\_e.swFeatureFilletKeepFeatures;

            //Create multiple-radius
fillets along selected edges
            swFeatMgr.**FeatureFillet**(FilletOptions,
0.01, (int)swFeatureFilletType\_e.swFeatureFilletType\_Simple,
(int)swFilletOverFlowType\_e.swFilletOverFlowType\_Default,
(VarRadArray8), 0, 0);

        }

        public
SldWorks
swApp;

    }
}