<!-- source: swdimxpertapi/Get_and_Set_Datum_Example_VB.htm -->

# SOLIDWORKS API Help

# Get and Set Datum Example (VBA)

This example shows how to get and set DimXpert datum
annotations.

'---------------------------------------------------------------------------
' Preconditions:
' 1. Open: *public\_documents***\samples\tutorial\dimxpert\bracket\_auto\_manual.sldprt.**
' 2. Select a face.
' 3. Open an Immediate window.
' 4. Ensure that the latest SOLIDWORKS DimXpert type library
is loaded:
'    a. click **Tools > References**.
'    b. Click Browse.
'    c. Find and select *install\_dir***\swdimxpert.tlb**.
'
' Postconditions:
' 1. Inspect the Immediate window.
' 2. Observe Plane1 and Datum G on the DimXpertManager tab.
'
' NOTE: Because this part is used elsewhere, do not save changes.
'--------------------------------------------------------------------------------------

Option Explicit
Dim dimXpertPart As dimXpertPart

Sub Main()

    Dim swapp As SldWorks.SldWorks
    Set swapp = Application.SldWorks
    Dim swModelDoc As SldWorks.ModelDoc2
    Set swModelDoc = swapp.ActiveDoc

   If swModelDoc Is Nothing Then
     Exit Sub
   End If

    Dim dimXpertMgr As
SldWorks.DimXpertManager
    Set dimXpertMgr =
swapp.IActiveDoc2.Extension.DimXpertManager(swapp.IActiveDoc2.IGetActiveConfiguration().Name,
True)
    Debug.Print "Model: " & swapp.IActiveDoc2.GetPathName

    Dim dimXpertPartObj As dimXpertPart

    Set dimXpertPartObj =
dimXpertMgr.dimXpertPart
    Set dimXpertPart = dimXpertPartObj

    Dim dimOption As DimXpertDimensionOption
    Set dimOption = dimXpertPart.**GetDimOption**
    dimOption.**DatumLength** = 0.06
    Dim dimarray(0) As Long
    dimarray(0) = 0
    Dim dimvar As Variant
    dimvar = dimarray
    dimOption.**FeatureSelectorOptions** = dimvar

    ' Insert datum
    dimXpertPart.**InsertDatum** dimOption

    Dim vAnnotations As Variant
    vAnnotations = dimXpertPart.GetAnnotations()

    Debug.Print "------------------------"
    Debug.Print "Annotations..."
    Debug.Print "------------------------"

    Dim annotationTemp As DimXpertAnnotation
    Dim annotationIndex As Long
    For annotationIndex = 0 To UBound(vAnnotations)
        Set annotationTemp =
vAnnotations(annotationIndex)
        Call AnnotationData(annotationTemp)
    Next

End Sub
Public Sub AnnotationData(annotation As DimXpertAnnotation)

    Dim annoType As Long

    'general info
    Call GeneralInfo(annotation)
    annoType = annotation.Type

    If annoType = swDimXpertDatum Then
        Call DatumData(annotation)

    End If

End Sub

Private Sub GeneralInfo(annotation As DimXpertAnnotation)

    Dim annoType As String
    Dim modelObj As Object
    Dim modelFeature As SldWorks.Feature

    Debug.Print ("")
    Debug.Print ("Name: " + annotation.Name)

    annoType =
annotationTypeNameFromObject(annotation)

    Debug.Print ("Type: " + annoType)
    Debug.Print ("Display Entity: " + DisplayEntity(annotation))

    Set modelObj = annotation.GetModelFeature
    Set modelFeature = modelObj

    If Not (modelFeature Is Nothing) Then
        Debug.Print ("ModelFeature: " +
modelFeature.Name + " (" + modelFeature.GetTypeName2() + ")")
    End If

End Sub

Private Sub DatumData(annotation As DimXpertDatum)

    ' the datum letter
    Debug.Print ("")
    Debug.Print ("Datum Letter:  " + annotation.**Identifier**)

End Sub

Private Function annotationTypeNameFromObject(anno As
DimXpertAnnotation) As String
    annotationTypeNameFromObject =
annotationTypeNameFromTypeNumber(anno.Type)
End Function

Private Function
annotationTypeNameFromTypeNumber(annoTypeIndex As Long) As String
    Select Case annoTypeIndex

    Case swDimXpertDimTol\_DistanceBetween
        annotationTypeNameFromTypeNumber = "DistanceBetween
Dim"
    Case swDimXpertDimTol\_CounterBore
        annotationTypeNameFromTypeNumber = "CounterBore
Dim"
    Case swDimXpertDimTol\_Depth
        annotationTypeNameFromTypeNumber =
"Depth Dim"
    Case swDimXpertDimTol\_CounterSinkDiameter
        annotationTypeNameFromTypeNumber = "CounterSinkDiameter
Dim"
    Case swDimXpertDimTol\_ChamferDimension
        annotationTypeNameFromTypeNumber = "ChamferDimension
Dim"
    Case swDimXpertDimTol\_AngleBetween
        annotationTypeNameFromTypeNumber = "AngleBetween
Dim"
    Case swDimXpertDimTol\_CounterSinkAngle
        annotationTypeNameFromTypeNumber = "CounterSinkAngle
Dim"
    Case swDimXpertDimTol\_ConeAngle
        annotationTypeNameFromTypeNumber = "ConeAngle
Dim"
    Case swDimXpertDimTol\_Diameter
        annotationTypeNameFromTypeNumber =
"Diameter Dim"
    Case swDimXpertDimTol\_Length
        annotationTypeNameFromTypeNumber =
"Length Dim"
    Case swDimXpertDimTol\_Radius
        annotationTypeNameFromTypeNumber =
"Radius Dim"
    Case swDimXpertDimTol\_Width
        annotationTypeNameFromTypeNumber =
"Width Dim"
    Case swDimXpertDimTol\_CompositeDistanceBetween
        annotationTypeNameFromTypeNumber = "CompositeDistanceBetween
Dim"

    Case swDimXpertDatum
        annotationTypeNameFromTypeNumber =
"Datum"

    Case swDimXpertGeoTol\_Position
        annotationTypeNameFromTypeNumber =
"Position Tol"
    Case swDimXpertGeoTol\_CompositePosition
        annotationTypeNameFromTypeNumber = "CompositePosition
Tol"
    Case swDimXpertGeoTol\_Symmetry
        annotationTypeNameFromTypeNumber =
"Symmetry Tol"
    Case swDimXpertGeoTol\_Concentricity
        annotationTypeNameFromTypeNumber =
"Concentricity Tol"
    Case swDimXpertGeoTol\_LineProfile
        annotationTypeNameFromTypeNumber = "LineProfile
Tol"
    Case swDimXpertGeoTol\_CompositeLineProfile
        annotationTypeNameFromTypeNumber = "CompositeLineProfile
Tol"
    Case swDimXpertGeoTol\_SurfaceProfile
        annotationTypeNameFromTypeNumber = "SurfaceProfile
Tol"
    Case swDimXpertGeoTol\_CompositeSurfaceProfile
        annotationTypeNameFromTypeNumber = "CompositeSurfaceProfile
Tol"
    Case swDimXpertGeoTol\_Angularity
        annotationTypeNameFromTypeNumber =
"Angularity Tol"
    Case swDimXpertGeoTol\_Parallelism
        annotationTypeNameFromTypeNumber =
"Parallelism Tol"
    Case swDimXpertGeoTol\_Perpendicularity
        annotationTypeNameFromTypeNumber =
"Perpendicularity Tol"
    Case swDimXpertGeoTol\_TotalRunout
        annotationTypeNameFromTypeNumber = "TotalRunout
Tol"
    Case swDimXpertGeoTol\_CircularRunout
        annotationTypeNameFromTypeNumber = "CircularRunout
Tol"
    Case swDimXpertGeoTol\_Flatness
        annotationTypeNameFromTypeNumber =
"Flatness Tol"
    Case swDimXpertGeoTol\_Circularity
        annotationTypeNameFromTypeNumber =
"Circularity Tol"
    Case swDimXpertGeoTol\_Cylindricity
        annotationTypeNameFromTypeNumber = "Cylindricity
Tol"
    Case swDimXpertGeoTol\_Straightness
        annotationTypeNameFromTypeNumber =
"Straightness Tol"
    Case swDimXpertGeoTol\_Tangency
        annotationTypeNameFromTypeNumber =
"Tangency Tol"
    Case Else
        annotationTypeNameFromTypeNumber =
"<unknown> " & CStr(annoTypeIndex)

    End Select

    ' returns a string containing the names of
the SW display entities
End Function
Private Function DisplayEntity(annotation As DimXpertAnnotation) As String

    Dim str As String
    Dim dispEnt As Object
    Dim swAnnot As SldWorks.annotation
    Set dispEnt = annotation.GetDisplayEntity
    If Not dispEnt Is Nothing Then
        If TypeOf dispEnt Is
SldWorks.annotation Then
            Set swAnnot =
dispEnt
            str =
swAnnot.GetName
        End If
    End If
    DisplayEntity = str
End Function