<!-- source: sldworksapi/Get_DimXpert_Display_Dimensions_and_Feature_Example_CSharp.htm -->

# SOLIDWORKS API Help

# Get DimXpert Display Dimensions and Feature Example (C#)

This example shows how to find out if an annotation is a DimXpert display
dimension, and, if so, how to get its DimXpert feature.

//----------------------------------------------------------------------------
// Preconditions:
// 1. Add **SolidWorks.Interop.swdimxpert.dll** as a reference
//    (in the Project Explorer, right-click **References**,
click **Add Reference,**
//    click **Browse**, and navigate to *install\_dir*\**api\redist**).
// 2. Open *public\_documents***\samples\tutorial\api\plate\_tolstatus.sldprt**.
// 3. Click **View > Toolbars > DimXpert**.
// 4. Click the **Auto Dimension Scheme** button on the DimXpert toolbar.
// 5. Verify that **Chamfer** and **Simple hole** are selected in Feature
Filters
//    in the Auto Dimension Scheme PropertyManager page and click
**OK**.
// 6. Open the Immediate window.
//
// Postconditions:
// 1. Gets the DimXpert display dimensions in the model.
// 2. Examine the Immediate window.
//
// NOTE: Because this part is used elsewhere, do not save changes.
//---------------------------------------------------------------------------

using SolidWorks.Interop.sldworks;
using SolidWorks.Interop.swconst;
using SolidWorks.Interop.swdimxpert;
using System;
using System.Diagnostics;

namespace Macro1CSharp.csproj

{

    partial class SolidWorksMacro

> {
>     public
> void Main()
>
>     {
>
>         ModelDoc2
> swPart = default(ModelDoc2);
>         Annotation
> swAnnotation = default(Annotation);
>         DisplayDimension
> swDisplayDimension = default(DisplayDimension);
>
>         swPart
> = (ModelDoc2)swApp.ActiveDoc;
>         swAnnotation
> = (Annotation)swPart.GetFirstAnnotation2();
>         while
> (((swAnnotation != null)))
>         {
>             Debug.Print("
> ");
>             Debug.Print("Annotation
> name = " + swAnnotation.GetName());
>             Debug.Print("Annotation
> DimXpert
> name = " + swAnnotation.GetDimXpertName());
>             int
> AnnotationType = (int)swDimensionType\_e.swDimensionTypeUnknown;
>             AnnotationType
> = swAnnotation.GetType();
>             if
> (AnnotationType == (int)swAnnotationType\_e.swDisplayDimension)
>             {
>                 Debug.Print("
> Is a display dimension? True");
>
>                 swDisplayDimension
> = (DisplayDimension)swAnnotation.GetSpecificAnnotation();
>                 switch
> ((swDisplayDimension.Type2))
>                 {
>                     case
> (int)swDimensionType\_e.swOrdinateDimension:
>                         Debug.Print("
> Display dimension type = base ordinate and its subordinates");
>                         break;
>                     case
> (int)swDimensionType\_e.swLinearDimension:
>                         Debug.Print("
> Display dimension type = linear");
>                         break;
>                     case
> (int)swDimensionType\_e.swAngularDimension:
>                         Debug.Print("
> Display dimension type  =
> angular");
>                         break;
>                     case
> (int)swDimensionType\_e.swArcLengthDimension:
>                         Debug.Print("
> Display dimension type = arc length");
>                         break;
>                     case
> (int)swDimensionType\_e.swRadialDimension:
>                         Debug.Print("
> Display dimension type = radial");
>                         break;
>                     case
> (int)swDimensionType\_e.swDiameterDimension:
>                         Debug.Print("
> Display dimension type = diameter");
>                         break;
>                     case
> (int)swDimensionType\_e.swHorOrdinateDimension:
>                         Debug.Print("
> Display dimension type = horizontal ordinate");
>                         break;
>                     case
> (int)swDimensionType\_e.swVertOrdinateDimension:
>                         Debug.Print("
> Display dimension type = vertical ordinate");
>                         break;
>                     case
> (int)swDimensionType\_e.swZAxisDimension:
>                         Debug.Print("
> Display dimension type = z-axis");
>                         break;
>                     case
> (int)swDimensionType\_e.swChamferDimension:
>                         Debug.Print("
> Display dimension type = chamfer dimension");
>                         break;
>                     case
> (int)swDimensionType\_e.swHorLinearDimension:
>                         Debug.Print("
> Display dimension type = horizontal linear");
>                         break;
>                     case
> (int)swDimensionType\_e.swVertLinearDimension:
>                         Debug.Print("
> Display dimension type = vertical linear");
>                         break;
>                     case
> (int)swDimensionType\_e.swScalarDimension:
>                         Debug.Print("
> Display dimension type = scalar");
>                         break;
>                     default:
>                         Debug.Print("
> Display dimension type = unknown");
>                         break;
>                 }
>                 Debug.Print("
> Is a DimXpert display dimension? " + (swDisplayDimension.IsDimXpert()
> == false ? "False" : "True"));
>                 if
> (swAnnotation.IsDimXpert())
>                 {
>                     DimXpertFeature
> DimXpertFeat = default(DimXpertFeature);
>                     string
> FeatName = null;
>
>                     DimXpertFeat
> = (DimXpertFeature)swAnnotation.GetDimXpertFeature();
>                     if
> ((DimXpertFeat != null))
>                     {
>                         FeatName
> = DimXpertFeat.Name;
>                         Debug.Print("
> DimXpert feature name = " + FeatName);
>                         switch
> ((DimXpertFeat.Type))
>                         {
>                             case
> swDimXpertFeatureType\_e.swDimXpertFeature\_Plane:
>                                 Debug.Print("
> DimXpert feature type = plane");
>                                 break;
>                             case
> swDimXpertFeatureType\_e.swDimXpertFeature\_Cylinder:
>                                 Debug.Print("
> DimXpert feature type = cylinder");
>                                 break;
>                             case
> swDimXpertFeatureType\_e.swDimXpertFeature\_Cone:
>                                 Debug.Print("
> DimXpert feature type = cone");
>                                 break;
>                             case
> swDimXpertFeatureType\_e.swDimXpertFeature\_Extrude:
>                                 Debug.Print("
> DimXpert feature type = extrude");
>                                 break;
>                             case
> swDimXpertFeatureType\_e.swDimXpertFeature\_Fillet:
>                                 Debug.Print("
> DimXpert feature type = fillet");
>                                 break;
>                             case
> swDimXpertFeatureType\_e.swDimXpertFeature\_Chamfer:
>                                 Debug.Print("
> DimXpert feature type = chamfer");
>                                 break;
>                             case
> swDimXpertFeatureType\_e.swDimXpertFeature\_CompoundHole:
>                                 Debug.Print("
> DimXpert feature type = compound hole");
>                                 break;
>                             case
> swDimXpertFeatureType\_e.swDimXpertFeature\_CompoundWidth:
>                                 Debug.Print("
> DimXpert feature type = compound width");
>                                 break;
>                             case
> swDimXpertFeatureType\_e.swDimXpertFeature\_CompoundNotch:
>                                 Debug.Print("
> DimXpert feature type = compound notch");
>                                 break;
>                             case
> swDimXpertFeatureType\_e.swDimXpertFeature\_CompoundClosedSlot3D:
>                                 Debug.Print("
> DimXpert feature type = compound closed-slot 3D");
>                                 break;
>                             case
> swDimXpertFeatureType\_e.swDimXpertFeature\_IntersectPoint:
>                                 Debug.Print("
> DimXpert feature type = intersect point");
>                                 break;
>                             case
> swDimXpertFeatureType\_e.swDimXpertFeature\_IntersectLine:
>                                 Debug.Print("
> DimXpert feature type = intersect line");
>                                 break;
>                             case
> swDimXpertFeatureType\_e.swDimXpertFeature\_IntersectCircle:
>                                 Debug.Print("
> DimXpert feature type = intersect circle");
>                                 break;
>                             case
> swDimXpertFeatureType\_e.swDimXpertFeature\_IntersectPlane:
>                                 Debug.Print("
> DimXpert feature type = intersect plane");
>                                 break;
>                             case
> swDimXpertFeatureType\_e.swDimXpertFeature\_Pattern:
>                                 Debug.Print("
> DimXpert feature type = pattern");
>                                 break;
>                             case
> swDimXpertFeatureType\_e.swDimXpertFeature\_Sphere:
>                                 Debug.Print("
> DimXpert feature type = sphere");
>                                 break;
>                             case
> swDimXpertFeatureType\_e.swDimXpertFeature\_BestfitPlane:
>                                 Debug.Print("
> DimXpert feature type = best-fit plane");
>                                 break;
>                             case
> swDimXpertFeatureType\_e.swDimXpertFeature\_Surface:
>                                 Debug.Print("
> DimXpert feature type = surface");
>                                 break;
>                             default:
>                                 Debug.Print("
> DimXpert feature type = unknown");
>                                 break;
>                         }
>                     }
>                 }
>             }
>             else
>             {
>                 Debug.Print("
> Not a display dimension.");
>             }
>             swAnnotation
> = (Annotation)swAnnotation.GetNext3();
>         }
>     }
>     ///
> <summary>
>     ///
> The SldWorks swApp variable is pre-assigned for you.
>     ///
> </summary>
>     public
> SldWorks swApp;
> }

}