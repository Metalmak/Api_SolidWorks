<!-- source: sldworksapi/Edit_Mate_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Edit Mate Example (C#)

This example shows how to edit an assembly mate.

//---------------------------------------------------------------------------
// Preconditions:
// 1. Open an assembly with a mate.
// 2. Select a mate.
// 3. Open the Immediate window.
//
// Postconditions:
// 1. Edits the selected assembly mate.
// 2. Examine the Immediate window.
//
// Note: Modifying a mate can cause mate errors.
//----------------------------------------------------------------------------
using
Microsoft.VisualBasic;
using
System;
using
System.Collections;
using
System.Collections.Generic;
using
System.Data;
using
System.Diagnostics;
using
SolidWorks.Interop.sldworks;
using
SolidWorks.Interop.swconst;
using
System.Runtime.InteropServices;

namespace
Macro1CSharp.csproj
{
    partial
class
SolidWorksMacro
    {

        public
bool
SelectMateEntity(SldWorks
swApp, ModelDoc2
swModel, MateEntity2
swMateEnt, int
nMark)
        {
            bool
functionReturnValue = false;

            Entity
swEnt = default(Entity);
            SelectionMgr
swSelMgr = default(SelectionMgr);
            SelectData
swSelData = default(SelectData);
            bool
bRet = false;

            switch
(swMateEnt.**ReferenceType**)
            {

                case
(int)swMateEntity2ReferenceType\_e.swMateEntity2ReferenceType\_Point:
                case
(int)swMateEntity2ReferenceType\_e.swMateEntity2ReferenceType\_Line:
                case
(int)swMateEntity2ReferenceType\_e.swMateEntity2ReferenceType\_Circle:
                case
(int)swMateEntity2ReferenceType\_e.swMateEntity2ReferenceType\_Plane:
                case
(int)swMateEntity2ReferenceType\_e.swMateEntity2ReferenceType\_Cylinder:
                case
(int)swMateEntity2ReferenceType\_e.swMateEntity2ReferenceType\_Sphere:
                case
(int)swMateEntity2ReferenceType\_e.swMateEntity2ReferenceType\_Cone:
                case
(int)swMateEntity2ReferenceType\_e.swMateEntity2ReferenceType\_SweptSurface:

                    swSelMgr = (SelectionMgr)swModel.**SelectionManager**;
                    swSelData = (SelectData)swSelMgr.**CreateSelectData**();
                    swEnt = (Entity)swMateEnt.**Reference**;

                    swSelData.**Mark** = nMark;

                    bRet = swEnt.**Select4**(true,
swSelData);

                    functionReturnValue = bRet;

                    return
functionReturnValue;

                case
(int)swMateEntity2ReferenceType\_e.swMateEntity2ReferenceType\_Set:
                case
(int)swMateEntity2ReferenceType\_e.swMateEntity2ReferenceType\_MultipleSurface:
                case
(int)swMateEntity2ReferenceType\_e.swMateEntity2ReferenceType\_GenSurface:
                case
(int)swMateEntity2ReferenceType\_e.swMateEntity2ReferenceType\_Ellipse:
                case
(int)swMateEntity2ReferenceType\_e.swMateEntity2ReferenceType\_GeneralCurve:
                case
(int)swMateEntity2ReferenceType\_e.swMateEntity2ReferenceType\_UNKNOWN:

                    break;

default:

                    break;
            }

            functionReturnValue = false;
            return
functionReturnValue;

        }

        public
void Main()
        {
            ModelDoc2
swModel = default(ModelDoc2);
            AssemblyDoc
swAssy = default(AssemblyDoc);
            SelectionMgr
swSelMgr = default(SelectionMgr);
            Feature
swFeat = default(Feature);
            Mate2
swMate = default(Mate2);
            DisplayDimension
swDispDim = default(DisplayDimension);
            Dimension
swDim = default(Dimension);
            string
sVarType = null;
            double
nVarFactor = 0;
            double
nMateDist = 0;
            int
nNumMateEnt = 0;
            MateEntity2
swMateEnt = null;
;
            double[]
vMateEntPar = null;
            Component2
swComp = default(Component2);
            int
nNewMateAlign = 0;
            int
nRetVal = 0;
            int
i = 0;
            bool
bRet = false;
            double[]
vDimValueArr = null;

            swModel = (ModelDoc2)swApp.**ActiveDoc**;
            swAssy = (AssemblyDoc)swModel;
            swSelMgr = (SelectionMgr)swModel.**SelectionManager**;
            swFeat = (Feature)swSelMgr.**GetSelectedObject6**(1,
-1);
            swMate = (Mate2)swFeat.**GetSpecificFeature2**();
            swDispDim = swMate.**get\_DisplayDimension2**(0);

            Debug.Print("File
= " + swModel.**GetPathName**());
            Debug.Print("  "
+ swFeat.**Name**);
            Debug.Print("    Type
= " + swMate.**Type**);
            Debug.Print("    Alignment      =
" + swMate.**Alignment**);
            Debug.Print("    CanBeFlipped
= " + swMate.**CanBeFlipped**);

            switch
(swMate.**Type**)
            {

                case
(int)swMateType\_e.swMateANGLE:

                    sVarType = " deg";

// radian = 180º/p
= 57.295779513º or approximately 57.3º
                    nVarFactor = 57.3;

                    break;
                case
(int)swMateType\_e.swMateDISTANCE:

                    sVarType = " mm";
                    nVarFactor = 1000.0;

                    break;
                case
(int)swMateType\_e.swMateGEAR:

                    sVarType = " ratio";
                    nVarFactor = 1.0;

                    break;
            }

            if
((int)swMateType\_e.swMateANGLE
== swMate.**Type** | (int)swMateType\_e.swMateDISTANCE
== swMate.**Type**)
            {
                Debug.Print("    MaxVar
= " + swMate.MaximumVariation \* nVarFactor
+ sVarType);
                Debug.Print("    MinVar
= " + swMate.MinimumVariation \* nVarFactor
+ sVarType);

            }

            if
((swDispDim != null))
            {
                swDim = (Dimension)swDispDim.**GetDimension**();
                vDimValueArr = (double[])swDim.**GetSystemValue3**((int)swInConfigurationOpts\_e.swThisConfiguration,
null);
                Debug.Print("    Dim
Value      = " + vDimValueArr[0] \*
nVarFactor + sVarType);

            }

            nNumMateEnt = swMate.**GetMateEntityCount**();

            for
(i = 0; i < nNumMateEnt; i++)
            {
                swMateEnt = swMate.**MateEntity**(i);
                swComp = swMateEnt.**ReferenceComponent**;

                vMateEntPar = (double[])swMateEnt.**EntityParams**;

                Debug.Print("      RefType("
+ i + ")   = "
+ swMateEnt.**ReferenceType**);
                Debug.Print("        Component          =
" + swComp.**Name2** +
" (" + swComp.**ReferencedConfiguration**
+ ") --> "
+ swComp.**GetPathName**());
                Debug.Print("        Point              =
(" + vMateEntPar[0] \* 1000.0 +
", " +
vMateEntPar[1] \* 1000.0 + ", "
+ vMateEntPar[2] \* 1000.0 + ") mm");
                Debug.Print("        Vector
= (" + vMateEntPar[3] +
", " +
vMateEntPar[4] + ", "
+ vMateEntPar[5] + ")");
                Debug.Print("        Radius
1           = " + vMateEntPar[6] \* 1000.0 +
" mm");
                Debug.Print("        Radius
2           = " + vMateEntPar[7] \* 1000.0 +
" mm");

            }

            switch
(swMate.**Type**)
            {

                case
(int)swMateType\_e.swMateGEAR:
                    // Cannot change
alignment on these mate types
                    return;
            }

            if
((int)swMateAlign\_e.swMateAlignALIGNED
== swMate.**Alignment**)
            {
                nNewMateAlign = (int)swMateAlign\_e.swMateAlignANTI\_ALIGNED;

            }
            else
            {
                if
((int)swMateAlign\_e.swMateAlignANTI\_ALIGNED
== swMate.**Alignment**)
                {
                    nNewMateAlign = (int)swMateAlign\_e.swMateAlignALIGNED;

                }
                else
                {
                    return;
                }
            }

            swModel.**ClearSelection2**(true);

            for
(i = 0; i <= nNumMateEnt - 1; i++)
            {
                //
IAssemblyDoc::EditMate3
requires that mate entities
                //
be selected with mark of 1 except for:
                //
swMateCAMFOLLOWER
                //
cam face              --> 1
                //
cam follower face     --> 8
                //
swMateSYMMETRIC
                //
symmetry faces        --> 1
                //
symmetry plane        --> 4

                bRet =
SelectMateEntity(swApp, swModel, swMate.**MateEntity**(i), 1);
            }

            //
IAssemblyDoc::EditMate3
requires mate feature to be selected last
            //
Mark is ignored
            bRet = swFeat.**Select2**(true,
0);

            swAssy.**EditMate3**(swMate.**Type**, nNewMateAlign,
true,
nMateDist, swMate.**MaximumVariation**, swMate.**MinimumVariation**,
0.0, 0.0, nMateDist, swMate.**MaximumVariation**,
            swMate.**MinimumVariation**,
false, true,
0, out
nRetVal);

            bRet = swModel.**EditRebuild3**();

        }

        public
SldWorks
swApp;

    }
}