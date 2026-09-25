<!-- source: swdimxpertapi/Get_and_Set_Datum_Example_VBNET.htm -->

# SOLIDWORKS API Help

# Get and Set Datum Example (VB.NET)

This example shows how to get
and set DimXpert datum annotations.

'---------------------------------------------------------------------------
' Preconditions:
' 1. Open *public\_documents***\samples\tutorial\dimxpert\bracket\_auto\_manual.sldprt.**
' 2. Select a face.
' 3. Open an Immediate window.
' 4. Ensure that the latest SOLIDWORKS DimXpert interop assembly is
referenced:
'    a. Right-click the project in Project Explorer.
'    b. Select **Add Reference**.
'    c. Click the Browse tab.
'    d. Find and select *install\_dir***\api\redist\swdimxpert.dll**.
'
' Postconditions:
' 1. Inspect the Immediate window.
' 2. Observe Plane1 and datum G on the DimXpertManager tab.
'
' NOTE: Because this part is used elsewhere, do not save changes.
'---------------------------------------------------------------------------
Imports
SolidWorks.Interop.sldworks
Imports
SolidWorks.Interop.swconst
Imports
SolidWorks.Interop.swdimxpert
Imports
System
Imports
System.Diagnostics

Partial
Class
SolidWorksMacro

    Dim
dimXpertPart As
dimXpertPart

    Sub
Main()

        Dim
swModelDoc As
ModelDoc2
        swModelDoc = swapp.ActiveDoc

        If
swModelDoc Is
Nothing
Then
            Exit
Sub
        End
If

        Dim
dimXpertMgr As
DimXpertManager
        dimXpertMgr =
swapp.IActiveDoc2.Extension.DimXpertManager(swapp.IActiveDoc2.IGetActiveConfiguration().Name,
True)
        Debug.Print("Model: "
& swapp.IActiveDoc2.GetPathName)

        Dim
dimXpertPartObj As
dimXpertPart

        dimXpertPartObj = dimXpertMgr.dimXpertPart
        dimXpertPart = dimXpertPartObj

        Dim
dimOption As
DimXpertDimensionOption
        dimOption = dimXpertPart.**GetDimOption**
        dimOption.**DatumLength** = 0.06
        Dim
dimarray(0) As
Long
        dimarray(0) = 0
        Dim
dimvar As
Object
        dimvar = dimarray
        dimOption.**FeatureSelectorOptions** = dimvar

        ' Insert datum
        dimXpertPart.**InsertDatum**(dimOption)

        Dim
vAnnotations As
Object
        vAnnotations =
dimXpertPart.GetAnnotations()

        Debug.Print("------------------------")
        Debug.Print("Annotations...")
        Debug.Print("------------------------")

        Dim
annotationTemp As
DimXpertAnnotation
        Dim
annotationIndex As
Long
        For
annotationIndex = 0 To
UBound(vAnnotations)
            annotationTemp = vAnnotations(annotationIndex)
            Call
AnnotationData(annotationTemp)
        Next

    End
Sub
    Public
Sub
AnnotationData(ByVal
annotation As
DimXpertAnnotation)

        Dim
annoType As
Long

        'general
info
        Call
GeneralInfo(annotation)
        annoType = annotation.Type

        If
annoType = swDimXpertAnnotationType\_e.swDimXpertDatum
Then
            Call
DatumData(annotation)

        End
If

    End
Sub

    Private
Sub
GeneralInfo(ByVal
annotation As
DimXpertAnnotation)

        Dim
annoType As
String
        Dim
modelObj As
Object
        Dim
modelFeature As
Feature

        Debug.Print("")
        Debug.Print("Name: "
+ annotation.Name)

        annoType = annotationTypeNameFromObject(annotation)

        Debug.Print("Type: "
+ annoType)
        Debug.Print("Display Entity: "
+ DisplayEntity(annotation))

        modelObj = annotation.GetModelFeature
        modelFeature = modelObj

        If
Not (modelFeature
Is
Nothing)
Then
            Debug.Print("ModelFeature:
" + modelFeature.Name +
" (" +
modelFeature.GetTypeName2() + ")")
        End
If

    End
Sub

    Private
Sub
DatumData(ByVal
annotation As
DimXpertDatum)

        ' the datum letter
        Debug.Print("")
        Debug.Print("Datum Letter:  "
+ annotation.**Identifier**)

    End
Sub

    Private
Function
annotationTypeNameFromObject(ByVal
anno As
DimXpertAnnotation) As
String
        annotationTypeNameFromObject =
annotationTypeNameFromTypeNumber(anno.Type)
    End
Function

    Private
Function
annotationTypeNameFromTypeNumber(ByVal
annoTypeIndex As
Long)
As
String
        Select
Case
annoTypeIndex

            Case
swDimXpertAnnotationType\_e.swDimXpertDimTol\_DistanceBetween
                annotationTypeNameFromTypeNumber =
"DistanceBetween Dim"
            Case
swDimXpertAnnotationType\_e.swDimXpertDimTol\_CounterBore
                annotationTypeNameFromTypeNumber =
"CounterBore Dim"
            Case
swDimXpertAnnotationType\_e.swDimXpertDimTol\_Depth
                annotationTypeNameFromTypeNumber =
"Depth Dim"
            Case
swDimXpertAnnotationType\_e.swDimXpertDimTol\_CounterSinkDiameter
                annotationTypeNameFromTypeNumber =
"CounterSinkDiameter Dim"
            Case
swDimXpertAnnotationType\_e.swDimXpertDimTol\_ChamferDimension
                annotationTypeNameFromTypeNumber =
"ChamferDimension Dim"
            Case
swDimXpertAnnotationType\_e.swDimXpertDimTol\_AngleBetween
                annotationTypeNameFromTypeNumber =
"AngleBetween Dim"
            Case
swDimXpertAnnotationType\_e.swDimXpertDimTol\_CounterSinkAngle
                annotationTypeNameFromTypeNumber =
"CounterSinkAngle Dim"
            Case
swDimXpertAnnotationType\_e.swDimXpertDimTol\_ConeAngle
                annotationTypeNameFromTypeNumber =
"ConeAngle Dim"
            Case
swDimXpertAnnotationType\_e.swDimXpertDimTol\_Diameter
                annotationTypeNameFromTypeNumber =
"Diameter Dim"
            Case
swDimXpertAnnotationType\_e.swDimXpertDimTol\_Length
                annotationTypeNameFromTypeNumber =
"Length Dim"
            Case
swDimXpertAnnotationType\_e.swDimXpertDimTol\_Radius
                annotationTypeNameFromTypeNumber =
"Radius Dim"
            Case
swDimXpertAnnotationType\_e.swDimXpertDimTol\_Width
                annotationTypeNameFromTypeNumber =
"Width Dim"
            Case
swDimXpertAnnotationType\_e.swDimXpertDimTol\_CompositeDistanceBetween
                annotationTypeNameFromTypeNumber =
"CompositeDistanceBetween Dim"

            Case
swDimXpertAnnotationType\_e.swDimXpertDatum
                annotationTypeNameFromTypeNumber =
"Datum"

            Case
swDimXpertAnnotationType\_e.swDimXpertGeoTol\_Position
                annotationTypeNameFromTypeNumber =
"Position Tol"
            Case
swDimXpertAnnotationType\_e.swDimXpertGeoTol\_CompositePosition
                annotationTypeNameFromTypeNumber =
"CompositePosition Tol"
            Case
swDimXpertAnnotationType\_e.swDimXpertGeoTol\_Symmetry
                annotationTypeNameFromTypeNumber =
"Symmetry Tol"
            Case
swDimXpertAnnotationType\_e.swDimXpertGeoTol\_Concentricity
                annotationTypeNameFromTypeNumber =
"Concentricity Tol"
            Case
swDimXpertAnnotationType\_e.swDimXpertGeoTol\_LineProfile
                annotationTypeNameFromTypeNumber =
"LineProfile Tol"
            Case
swDimXpertAnnotationType\_e.swDimXpertGeoTol\_CompositeLineProfile
                annotationTypeNameFromTypeNumber =
"CompositeLineProfile Tol"
            Case
swDimXpertAnnotationType\_e.swDimXpertGeoTol\_SurfaceProfile
                annotationTypeNameFromTypeNumber =
"SurfaceProfile Tol"
            Case
swDimXpertAnnotationType\_e.swDimXpertGeoTol\_CompositeSurfaceProfile
                annotationTypeNameFromTypeNumber =
"CompositeSurfaceProfile Tol"
            Case
swDimXpertAnnotationType\_e.swDimXpertGeoTol\_Angularity
                annotationTypeNameFromTypeNumber =
"Angularity Tol"
            Case
swDimXpertAnnotationType\_e.swDimXpertGeoTol\_Parallelism
                annotationTypeNameFromTypeNumber =
"Parallelism Tol"
            Case
swDimXpertAnnotationType\_e.swDimXpertGeoTol\_Perpendicularity
                annotationTypeNameFromTypeNumber =
"Perpendicularity Tol"
            Case
swDimXpertAnnotationType\_e.swDimXpertGeoTol\_TotalRunout
                annotationTypeNameFromTypeNumber =
"TotalRunout Tol"
            Case
swDimXpertAnnotationType\_e.swDimXpertGeoTol\_CircularRunout
                annotationTypeNameFromTypeNumber =
"CircularRunout Tol"
            Case
swDimXpertAnnotationType\_e.swDimXpertGeoTol\_Flatness
                annotationTypeNameFromTypeNumber =
"Flatness Tol"
            Case
swDimXpertAnnotationType\_e.swDimXpertGeoTol\_Circularity
                annotationTypeNameFromTypeNumber =
"Circularity Tol"
            Case
swDimXpertAnnotationType\_e.swDimXpertGeoTol\_Cylindricity
                annotationTypeNameFromTypeNumber =
"Cylindricity Tol"
            Case
swDimXpertAnnotationType\_e.swDimXpertGeoTol\_Straightness
                annotationTypeNameFromTypeNumber =
"Straightness Tol"
            Case
swDimXpertAnnotationType\_e.swDimXpertGeoTol\_Tangency
                annotationTypeNameFromTypeNumber =
"Tangency Tol"
            Case
Else
                annotationTypeNameFromTypeNumber
= "<unknown> "
& CStr(annoTypeIndex)

        End
Select

    End
Function
    Private
Function
DisplayEntity(ByVal
annotation As
DimXpertAnnotation) As
String

        Dim
str As
String
        Dim
dispEnt As
Object
        Dim
swAnnot As
Annotation
        str = Nothing
        dispEnt =
annotation.GetDisplayEntity
        If
Not dispEnt
Is
Nothing
Then
            If
TypeOf
dispEnt Is
Annotation Then
                swAnnot = dispEnt
                str = swAnnot.GetName
            End
If
        End
If
        DisplayEntity = str
    End
Function

    Public
swApp As
SldWorks

End
Class