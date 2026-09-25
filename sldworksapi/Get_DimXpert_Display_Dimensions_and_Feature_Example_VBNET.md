<!-- source: sldworksapi/Get_DimXpert_Display_Dimensions_and_Feature_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Get DimXpert Display Dimensions and Feature Example (VB.NET)

This example shows how to find out if an annotation is a DimXpert display
dimension, and, if so, how to get its DimXpert feature.

'----------------------------------------------------------------------------
' Preconditions:
' 1. Add **SolidWorks.Interop.swdimxpert.dll** as a reference
'    (in the Project Explorer, right-click **References**,
click **Add Reference,**
'    click **Browse**, and navigate to *install\_dir*\**api\redist**).
' 2. Open *public\_documents***\samples\tutorial\api\plate\_tolstatus.sldprt**.
' 3. Click **View > Toolbars > DimXpert**.
' 4. Click the **Auto Dimension Scheme** button on the DimXpert toolbar.
' 5. Verify that **Chamfer** and **Simple hole** are selected in Feature
Filters
'    in the Auto Dimension Scheme PropertyManager page and click
**OK**.
' 6. Open the Immediate window.
'
' Postconditions:
' 1. Gets the DimXpert display dimensions in the model.
' 2. Examine the Immediate window.
'
' NOTE: Because this part is used elsewhere, do not save changes.
'---------------------------------------------------------------------------

Imports SolidWorks.Interop.sldworks
Imports SolidWorks.Interop.swconst
Imports SolidWorks.Interop.swdimxpert
Imports System
Imports System.Diagnostics

Partial Class SolidWorksMacro

    Public
Sub Main()

        Dim
swPart As ModelDoc2
        Dim
swAnnotation As Annotation
        Dim
swDisplayDimension As DisplayDimension

        swPart
= swApp.ActiveDoc
        swAnnotation
= swPart.GetFirstAnnotation2
        Do
While (Not (swAnnotation Is Nothing))
            Debug.Print("
")
            Debug.Print("Annotation
name = " & swAnnotation.GetName)
            Debug.Print("Annotation
DimXpert
name = " & swAnnotation.GetDimXpertName)
            If
swAnnotationType\_e.swDisplayDimension = swAnnotation.GetType
Then
                Debug.Print("
 Is a display
dimension? True")
                swDisplayDimension
= swAnnotation.GetSpecificAnnotation
                Select
Case (swDisplayDimension.Type2)
                    Case
swDimensionType\_e.swOrdinateDimension
                        Debug.Print("
 Display
dimension type = base ordinate and its subordinates")
                    Case
swDimensionType\_e.swLinearDimension
                        Debug.Print("
 Display
dimension type = linear")
                    Case
swDimensionType\_e.swAngularDimension
                        Debug.Print("
 Display
dimension type  =
angular")
                    Case
swDimensionType\_e.swArcLengthDimension
                        Debug.Print("
 Display
dimension type = arc length")
                    Case
swDimensionType\_e.swRadialDimension
                        Debug.Print("
 Display
dimension type = radial")
                    Case
swDimensionType\_e.swDiameterDimension
                        Debug.Print("
 Display
dimension type = diameter")
                    Case
swDimensionType\_e.swHorOrdinateDimension
                        Debug.Print("
 Display
dimension type = horizontal ordinate")
                    Case
swDimensionType\_e.swVertOrdinateDimension
                        Debug.Print("
 Display
dimension type = vertical ordinate")
                    Case
swDimensionType\_e.swZAxisDimension
                        Debug.Print("
 Display
dimension type = z-axis")
                    Case
swDimensionType\_e.swChamferDimension
                        Debug.Print("
 Display
dimension type = chamfer dimension")
                    Case
swDimensionType\_e.swHorLinearDimension
                        Debug.Print("
 Display
dimension type = horizontal linear")
                    Case
swDimensionType\_e.swVertLinearDimension
                        Debug.Print("
 Display
dimension type = vertical linear")
                    Case
swDimensionType\_e.swScalarDimension
                        Debug.Print("
 Display
dimension type = scalar")
                    Case
Else
                        Debug.Print("
 Display
dimension type = unknown")
                End
Select
                Debug.Print("
 Is a DimXpert
display dimension? " & IIf(swDisplayDimension.IsDimXpert
= False, "False", "True"))
                If
swAnnotation.IsDimXpert Then
                    Dim
DimXpertFeat As DimXpertFeature
                    Dim
FeatName As String
                    DimXpertFeat
= swAnnotation.GetDimXpertFeature()
                    If
Not DimXpertFeat Is Nothing Then
                        FeatName
= DimXpertFeat.Name
                        Debug.Print("
 DimXpert
feature name = " & FeatName)
                        Select
Case (DimXpertFeat.Type)
                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_Plane
                                Debug.Print("
 DimXpert
feature type = plane")
                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_Cylinder
                                Debug.Print("
 DimXpert
feature type = cylinder")
                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_Cone
                                Debug.Print("
 DimXpert
feature type = cone")
                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_Extrude
                                Debug.Print("
 DimXpert
feature type = extrude")
                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_Fillet
                                Debug.Print("
 DimXpert
feature type = fillet")
                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_Chamfer
                                Debug.Print("
 DimXpert
feature type = chamfer")
                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_CompoundHole
                                Debug.Print("
 DimXpert
feature type = compound hole")
                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_CompoundWidth
                                Debug.Print("
 DimXpert
feature type = compound width")
                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_CompoundNotch
                                Debug.Print("
 DimXpert
feature type = compound notch")
                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_CompoundClosedSlot3D
                                Debug.Print("
 DimXpert
feature type = compound closed-slot 3D")
                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_IntersectPoint
                                Debug.Print("
 DimXpert
feature type = intersect point")
                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_IntersectLine
                                Debug.Print("
 DimXpert
feature type = intersect line")
                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_IntersectCircle
                                Debug.Print("
 DimXpert
feature type = intersect circle")
                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_IntersectPlane
                                Debug.Print("
 DimXpert
feature type = intersect plane")
                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_Pattern
                                Debug.Print("
 DimXpert
feature type = pattern")
                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_Sphere
                                Debug.Print("
 DimXpert
feature type = sphere")
                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_BestfitPlane
                                Debug.Print("
 DimXpert
feature type = best-fit plane")
                            Case
swDimXpertFeatureType\_e.swDimXpertFeature\_Surface
                                Debug.Print("
 DimXpert
feature type = surface")
                            Case
Else
                                Debug.Print("
 DimXpert
feature type = unknown")
                        End
Select
                    End
If
                End
If
            Else
                Debug.Print("
 Not a display
dimension.")
            End
If
            swAnnotation
= swAnnotation.GetNext3
        Loop
    End
Sub

    '''
<summary>
    '''
The SldWorks swApp variable is pre-assigned for you.
    '''
</summary>
    Public
swApp As SldWorks

End Class