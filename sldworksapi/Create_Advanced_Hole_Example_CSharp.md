<!-- source: sldworksapi/Create_Advanced_Hole_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Create Advanced Hole Feature Example (C#)

This example shows how to create an Advanced Hole feature.

//----------------------------------------------------------------------------

// Preconditions:
// 1. Verify that the specified part document exists.
// 2. Open the Immediate window.
//
// Postconditions:
// 1. Selects near and far side faces of the Advanced Hole.
// 2. Defines an Advanced Hole at a sketch point on the edge of the block
//    with the following:
//    \* Countersink near side element
//    \* Straight tap near side element
//    \* Counterbore far side element
//    \* Straight hole far side element
// 3. Gets some near and far side element data for the Advanced Hole.
// 4. Modifies the near side element array to contain a tapered tap element.
// 5. Deletes the Advanced Hole's defining sketch point on the edge of the
block.
// 6. Adds two sketch points and creates two Advanced Holes at those locations
//    using the previously defined Advanced Hole.
// 7. Inspect the Immediate window and graphics area.
//
// NOTE: Because the model is used elsewhere, do not save changes.
//----------------------------------------------------------------------------

using SolidWorks.Interop.sldworks;
using SolidWorks.Interop.swconst;
using System.Diagnostics;
using System.Runtime.InteropServices;

namespace CreateAdvancedHole\_CSharp
{
    public partial class SolidWorksMacro
    {
        public void Main()
        {

            ModelDoc2 swModel = default(ModelDoc2);
            Feature feat = default(Feature);
            bool boolstatus = false;
            AdvancedHoleElementData swAdvHole\_Near\_1 = default(AdvancedHoleElementData);
            AdvancedHoleElementData swAdvHole\_Near\_2 = default(AdvancedHoleElementData);
            AdvancedHoleElementData swAdvHole\_Near\_3 = default(AdvancedHoleElementData);
            AdvancedHoleElementData swAdvHole\_Far\_1 = default(AdvancedHoleElementData);
            AdvancedHoleElementData swAdvHole\_Far\_2 = default(AdvancedHoleElementData);
            CountersinkElementData swCounterSinkNear = default(CountersinkElementData);
            CounterboreElementData swCounterBoreFar = default(CounterboreElementData);
            StraightElementData swStraightHoleFar = default(StraightElementData);
            StraightTapElementData swStraightTapNear = default(StraightTapElementData);
            TaperedTapElementData swTaperedTapNear = default(TaperedTapElementData);
            FeatureManager swFeatureMgr = default(FeatureManager);
            double ConvFactorLength = 0;
            AdvancedHoleElementData[] advHoleNearArr = new AdvancedHoleElementData[2];
            AdvancedHoleElementData[] advHoleFarArr = new AdvancedHoleElementData[2];
            AdvancedHoleFeatureData featdata = default(AdvancedHoleFeatureData);
            AdvancedHoleElementData[] newNearArr = new AdvancedHoleElementData[2];
            AdvancedHoleElementData[] newFarArr = new AdvancedHoleElementData[2];
            Feature swSketchFeature = default(Feature);
            SelectionMgr swSelectionManager = default(SelectionMgr);
            Sketch swSketch = default(Sketch);
            object[] swSketchPointArray = null;
            int swMaxPointNumber = 0;
            object skPoint = null;
            object swSketchPoint = null;
            int swCurrentPointNumber = 0;
            int errors = 0;
            int warnings = 0;
            object ResultArray = null;
            string CalloutString = null;
            string StrDiam = null;
            string strDepth = null;
            object[] nearSide = null;
            object[] farSide = null;

            bool retval = false;

            swModel = swApp.**OpenDoc6**("C:\\Users\\Public\\Documents\\SOLIDWORKS\\SOLIDWORKS 2018\\samples\\tutorial\\api\\block20.sldprt", (int)swDocumentTypes\_e.swDocPART, (int)swOpenDocOptions\_e.swOpenDocOptions\_Silent, "", ref errors, ref warnings);
            swFeatureMgr = swModel.**FeatureManager**;

            //Conversion from inches to meters
            ConvFactorLength = 25.4 / 1000;

            //Select two faces for the near side and far side hole elements
            boolstatus = swModel.**Extension**.**SelectByRay**(-0.0589202612791269, 0.0260626824463657, 0.0560000000000969, -0.400036026779312, -0.515038074910024, -0.758094294050284, 0.000722831189342222, 2, false, 256,
            0);
            //Near side
            boolstatus = swModel.**Extension**.**SelectByRay**(-0.0110716643645077, 0.0211784489308116, -0.0639370439421896, 0.18261953966356, -0.612697461661826, 0.76892907618728, 0.000936301020408163, 2, false, 512,
            0);
            //Far side

            //Define near and far side hole elements

            //Near side countersink
            swAdvHole\_Near\_1 = (AdvancedHoleElementData)swModel.**Extension**.**CreateAdvancedHoleElementData**((int)swAdvWzdGeneralHoleTypes\_e.swAdvWzdCounterSink);

            swAdvHole\_Near\_1.**Orientation** = (int)swHoleElementOrientation\_e.swHoleElementOrientation\_Nearside;
            swAdvHole\_Near\_1.**Size** = "#4";
            swAdvHole\_Near\_1.**Standard** = 0;
            swAdvHole\_Near\_1.**FastenerType** = (int)swWzdHoleStandardFastenerTypes\_e.swStandardAnsiInchFlatHead100;
            swAdvHole\_Near\_1.**Diameter** = ConvFactorLength \* 0.225;
            swAdvHole\_Near\_1.**BlindDepth** = 0.02055794 \* ConvFactorLength;
            swAdvHole\_Near\_1.**EndCondition** = (int)swEndConditions\_e.swEndCondBlind;
            swCounterSinkNear = (CountersinkElementData)swAdvHole\_Near\_1;
            swCounterSinkNear.**EndConditionOverride** = true;
            swCounterSinkNear.**AngleOverride** = false;

            //Near side straight tap
            swAdvHole\_Near\_2 = (AdvancedHoleElementData)swModel.**Extension**.**CreateAdvancedHoleElementData**((int)swAdvWzdGeneralHoleTypes\_e.swAdvWzdStraightTap);

            swAdvHole\_Near\_2.**Size** = "#4-40";
            swAdvHole\_Near\_2.**Standard** = (int)swWzdHoleStandards\_e.swStandardAnsiInch;
            swAdvHole\_Near\_2.**FastenerType** = (int)swWzdHoleStandardFastenerTypes\_e.swStandardAnsiInchBottomingTappedHole;
            swAdvHole\_Near\_2.**Diameter** = ConvFactorLength \* 0.089;
            swAdvHole\_Near\_2.**EndCondition** = (int)swEndConditions\_e.swEndCondUpToNext;
            swAdvHole\_Near\_2.**DiameterOverride** = true;
            swStraightTapNear = (StraightTapElementData)swAdvHole\_Near\_2;
            swStraightTapNear.**CustomSizing** = (int)swStraightTapHoleCustomSizing\_e.swStraightTapHoleCustomSizing\_TapDrillDiameter;
            swStraightTapNear.**ThreadClass** = (int)swStraightTapHoleThreadClass\_e.swStraightTapHoleThreadClass\_1B;
            swStraightTapNear.**ThreadClassOverride** = true;

            //Near side tapered tap
            swAdvHole\_Near\_3 = (AdvancedHoleElementData)swModel.**Extension**.**CreateAdvancedHoleElementData**((int)swAdvWzdGeneralHoleTypes\_e.swAdvWzdTaperTap);

            swAdvHole\_Near\_3.**Orientation** = (int)swHoleElementOrientation\_e.swHoleElementOrientation\_Nearside;
            swAdvHole\_Near\_3.**Size** = "1/16";
            swAdvHole\_Near\_3.**Standard** = (int)swWzdHoleStandards\_e.swStandardAnsiInch;
            swAdvHole\_Near\_3.**FastenerType** = (int)swWzdHoleStandardFastenerTypes\_e.swStandardAnsiInchTaperedPipeTap;
            swAdvHole\_Near\_3.**Diameter** = ConvFactorLength \* 0.266;
            swAdvHole\_Near\_2.**BlindDepth** = 0.205 \* ConvFactorLength;
            swAdvHole\_Near\_3.**EndCondition** = (int)swEndConditions\_e.swEndCondBlind;
            swAdvHole\_Near\_3.**DiameterOverride** = true;
            swTaperedTapNear = (TaperedTapElementData)swAdvHole\_Near\_3;
            swTaperedTapNear.**CustomSizing** = (int)swTaperedTapCustomSizing\_e.swTaperedTapCustomSizing\_MinorDiameterWithCosmeticThread;
            swTaperedTapNear.**ThreadClass** = (int)swTaperedTapThreadClass\_e.swTaperedTapThreadClass\_1;
            swTaperedTapNear.**ThreadClassOverride** = true;
            swTaperedTapNear.**EndConditionOverride** = true;

            //Far side counterbore
            swAdvHole\_Far\_1 = (AdvancedHoleElementData)swModel.**Extension**.**CreateAdvancedHoleElementData**((int)swAdvWzdGeneralHoleTypes\_e.swAdvWzdCounterBore);

            swAdvHole\_Far\_1.**Orientation** = (int)swHoleElementOrientation\_e.swHoleElementOrientation\_Farside;
            swAdvHole\_Far\_1.**Size** = "#8";
            swAdvHole\_Far\_1.**Standard** = (int)swWzdHoleStandards\_e.swStandardAnsiInch;
            swAdvHole\_Far\_1.**FastenerType** = (int)swWzdHoleStandardFastenerTypes\_e.swStandardAnsiInchBinding;
            swAdvHole\_Far\_1.**Diameter** = ConvFactorLength \* 0.375;
            swAdvHole\_Far\_1.**BlindDepth** = 0.105 \* ConvFactorLength;
            swAdvHole\_Far\_1.**EndCondition** = (int)swEndConditions\_e.swEndCondBlind;
            swAdvHole\_Far\_1.**DiameterOverride** = true;
            swCounterBoreFar = (CounterboreElementData)swAdvHole\_Far\_1;
            swCounterBoreFar.**EndConditionOverride** = true;

            //Far side straight
            swAdvHole\_Far\_2 = (AdvancedHoleElementData)swModel.**Extension**.**CreateAdvancedHoleElementData**((int)swAdvWzdGeneralHoleTypes\_e.swAdvWzdStraight);

            swAdvHole\_Far\_2.**Size** = "1/16";
            swAdvHole\_Far\_2.**Standard** = 0;
            swAdvHole\_Far\_2.**FastenerType** = (int)swWzdHoleStandardFastenerTypes\_e.swStandardAnsiInchAllDrillSizes;
            swAdvHole\_Far\_2.**Diameter** = ConvFactorLength \* 0.0625;
            swAdvHole\_Far\_2.**BlindDepth** = 0.2711 \* ConvFactorLength;
            swAdvHole\_Far\_2.**EndCondition** = (int)swEndConditions\_e.swEndCondBlind;
            swAdvHole\_Far\_2.**DiameterOverride** = true;

            //Customize the hole callout for this straight element
            StrDiam = swModel.Extension.**GetCalloutVariableString**((int)swCalloutVariable\_e.swCalloutVariable\_AH\_Straight\_Diameter);
            strDepth = swModel.Extension.**GetCalloutVariableString**((int)swCalloutVariable\_e.swCalloutVariable\_AH\_Straight\_Depth);
            CalloutString = "<MOD-DIAM> " + StrDiam + " " + "<HOLE-DEPTH> " + strDepth;
            swAdvHole\_Far\_2.**CalloutString** = CalloutString;

            swStraightHoleFar = (StraightElementData)swAdvHole\_Far\_2;

            //Set near and far side element arrays
            advHoleNearArr[0] = (AdvancedHoleElementData)swCounterSinkNear;
            advHoleNearArr[1] = (AdvancedHoleElementData)swStraightTapNear;
            advHoleFarArr[0] = (AdvancedHoleElementData)swCounterBoreFar;
            advHoleFarArr[1] = (AdvancedHoleElementData)swStraightHoleFar;

```
	    DispatchWrapper[] dispArray = ObjectArrayToDispatchWrapperArray(new object[] { advHoleNearArr[0], advHoleNearArr[1] });
            DispatchWrapper[] dispArray2 = ObjectArrayToDispatchWrapperArray(new object[] { advHoleFarArr[0], advHoleFarArr[1] });

            //Create the Advanced Hole using the near and far side element arrays; specify to not use baseline dimensions; customize Hole Callouts

            feat = swFeatureMgr.AdvancedHole2(dispArray, dispArray2, false, true, false, out ResultArray);

            //Get some near and far side element data

            featdata = (AdvancedHoleFeatureData)feat.GetDefinition();

            featdata.AccessSelections(swModel, null);

            Debug.Print("Number of near side hole elements: " + featdata.NearSideElementsCount);

            Debug.Print("Number of far side hole elements: " + featdata.FarSideElementsCount);

            nearSide = (object[])featdata.GetNearSideElements();

            swCounterSinkNear = (CountersinkElementData)nearSide[0];

            farSide = (object[])featdata.GetFarSideElements();

            swCounterBoreFar = (CounterboreElementData)farSide[0];

            swStraightHoleFar = (StraightElementData)farSide[1];

            Debug.Print("Near side countersink:");

            Debug.Print("   Hole element type as defined in swAdvWzdGeneralHoleTypes_e: " + ((AdvancedHoleElementData)swCounterSinkNear).ElementType);

            Debug.Print("   Size as defined on the Advanced Hole PropertyManager page: " + ((AdvancedHoleElementData)swCounterSinkNear).Size);

            Debug.Print("   Standard as defined in swWzdHoleStandards_e: " + ((AdvancedHoleElementData)swCounterSinkNear).Standard);

            Debug.Print("   Fastener type as defined in swWzdHoleStandardFastenerTypes_e: " + ((AdvancedHoleElementData)swCounterSinkNear).FastenerType);

            Debug.Print("   Diameter in m: " + ((AdvancedHoleElementData)swCounterSinkNear).Diameter);

            Debug.Print("   Blind depth in m: " + ((AdvancedHoleElementData)swCounterSinkNear).BlindDepth);

            Debug.Print("   Orientation as defined in swHoleElementOrientation_e: " + ((AdvancedHoleElementData)swCounterSinkNear).Orientation);

            Debug.Print("   End condition as defined in swEndConditions_e: " + ((AdvancedHoleElementData)swCounterSinkNear).EndCondition);

            Debug.Print("Far side straight:");

            Debug.Print("   Hole element type as defined in swAdvWzdGeneralHoleTypes_e: " + ((AdvancedHoleElementData)swStraightHoleFar).ElementType);

            Debug.Print("   Size as defined on the Advanced Hole PropertyManager page: " + ((AdvancedHoleElementData)swStraightHoleFar).Size);

            Debug.Print("   Standard as defined in swWzdHoleStandards_e: " + ((AdvancedHoleElementData)swStraightHoleFar).Standard);

            Debug.Print("   Fastener type as defined in swWzdHoleStandardFastenerTypes_e: " + ((AdvancedHoleElementData)swStraightHoleFar).FastenerType);

            Debug.Print("   Diameter in m: " + ((AdvancedHoleElementData)swStraightHoleFar).Diameter);

            Debug.Print("   Diameter override? " + ((AdvancedHoleElementData)swStraightHoleFar).DiameterOverride);

            Debug.Print("   Blind depth in m: " + ((AdvancedHoleElementData)swStraightHoleFar).BlindDepth);

            Debug.Print("   End condition as defined in swEndConditions_e: " + ((AdvancedHoleElementData)swStraightHoleFar).EndCondition);

            Debug.Print("   Customized hole callout: " + ((AdvancedHoleElementData)swStraightHoleFar).CalloutString);

            //Modify the near and far side element arrays

            newNearArr[0] = (AdvancedHoleElementData)swTaperedTapNear;

            newNearArr[1] = (AdvancedHoleElementData)swStraightTapNear;

            //newFarArr[0] = (AdvancedHoleElementData)swCounterBoreFar;

            //newFarArr[1] = (AdvancedHoleElementData)swStraightHoleFar;

            featdata.SetNearSideElements(newNearArr);

            //featdata.SetFarSideElements(newFarArr);

            feat.ModifyDefinition(featdata, swModel, null);

            //Delete the first point used to define the Advanced Hole

            swSketchFeature = (Feature)feat.GetFirstSubFeature();

            swSketchFeature.Select2(false, 0);

            swModel.EditSketch();

            swSelectionManager = (SelectionMgr)swModel.SelectionManager;

            swSketch = (Sketch)swSketchFeature.GetSpecificFeature2();

            swSketchPointArray = (object[])swSketch.GetSketchPoints2();

            swMaxPointNumber = swSketchPointArray.GetUpperBound(0);

            for (swCurrentPointNumber = 0; swCurrentPointNumber <= swMaxPointNumber; swCurrentPointNumber += 1)

            {

                swSketchPoint = swSketchPointArray[swCurrentPointNumber];

                retval = swSelectionManager.AddSelectionListObject(swSketchPoint, null);

                swModel.EditDelete();

            }

            //Create points for multiple Advanced Hole locations

            skPoint = swModel.SketchManager.CreatePoint(-0.0319158789518497, 0.0344489966898323, 0.05600000000004);

            skPoint = swModel.SketchManager.CreatePoint(-0.0494104502066557, 0.0080156770060853, 0.0560000000000969);

            swModel.SketchManager.InsertSketch(true);

        }
```

```
	public DispatchWrapper[] ObjectArrayToDispatchWrapperArray(object[] Objects)
        {
            int ArraySize = 0;
            ArraySize = Objects.GetUpperBound(0);
            DispatchWrapper[] d = new DispatchWrapper[ArraySize + 1];
            int ArrayIndex = 0;
            for (ArrayIndex = 0; ArrayIndex <= ArraySize; ArrayIndex++)
            {;
                d[ArrayIndex] = new DispatchWrapper(Objects[ArrayIndex]);
            }
            return d;
        }
```

```

        // The SldWorks swApp variable is pre-assigned for you.

        public SldWorks swApp;

    }

}
```