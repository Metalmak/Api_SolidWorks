<!-- source: sldworksapi/Get_All_Sheet_Metal_Feature_Data_Example_VB.htm -->

# SOLIDWORKS API Help

# Get All Sheet Metal Feature Data Example (VBA)

This example shows how to get all of the sheet metal part's feature
data.

```
'------------------------------------------------
' Preconditions:
' 1. Open a sheet metal part.
' 2. Open the Immediate window.
'
' Postconditions: Inspect the Immediate window.
'------------------------------------------------
Dim swApp As SldWorks.SldWorks
Dim swSelMgr As SldWorks.SelectionMgr
Dim swFeat As SldWorks.Feature
Dim swSubFeat As SldWorks.Feature
Dim bRet As Boolean
Dim lRet As Long
Dim gaugeTableFile As String
```

Option Explicit

Sub Process\_CustomBendAllowance \_
( \_
    swApp As SldWorks.SldWorks, \_
    swModel As SldWorks.ModelDoc2, \_
    swCustBend As SldWorks.CustomBendAllowance \_
)

    Debug.Print "
BendAllowance    = " & swCustBend.**BendAllowance** \* 1000# &
" mm"
    Debug.Print "      BendDeduction
= " & swCustBend.**BendDeduction** \* 1000# & " mm"
    Debug.Print "      BendTableFile
= " & swCustBend.**BendTableFile**
    Debug.Print "      KFactor
= " & swCustBend.**KFactor**
    Debug.Print "      Type
= " & swCustBend.**Type**

End Sub

Sub Process\_SMBaseFlange \_
( \_
    swApp As SldWorks.SldWorks, \_
    swModel As SldWorks.ModelDoc2, \_
    swFeat As SldWorks.Feature \_
)

    Debug.Print "  +" & swFeat.**Name**
& " [" & swFeat.**GetTypeName** & "]"

    Dim swBaseFlange
As SldWorks.BaseFlangeFeatureData
    Set swBaseFlange = swFeat.**GetDefinition**

    Debug.Print "    BendRadius
= " & swBaseFlange.**BendRadius** \* 1000# & " mm"

End Sub

Sub Process\_SheetMetal \_
( \_
    swApp As SldWorks.SldWorks, \_
    swModel As SldWorks.ModelDoc2, \_
    swFeat As SldWorks.Feature \_
)

    Debug.Print "  +" & swFeat.**Name**
& " [" & swFeat.**GetTypeName** & "]"

    Dim swSheetMetal  As
SldWorks.SheetMetalFeatureData
    Set swSheetMetal = swFeat.**GetDefinition**

    Dim swCustBend As SldWorks.**CustomBendAllowance**
    Set swCustBend = swSheetMetal.**GetCustomBendAllowance**
    Debug.Print "    BendRadius = " &
swSheetMetal.**BendRadius** \* 1000# & " mm"

    Process\_CustomBendAllowance swApp, swModel,
swCustBend

    lRet = swSheetMetal.**GetUseGaugeTable**(bRet,
gaugeTableFile)
    Debug.Print "    Use gauge table? " & bRet
    Debug.Print "      Error code as
defined in swSheetMetalModifierError\_e: " & lRet

End Sub

Sub Process\_SM3dBend \_
( \_
    swApp As SldWorks.SldWorks, \_
    swModel As SldWorks.ModelDoc2, \_
    swFeat As SldWorks.Feature \_
)

    Debug.Print "  +" & swFeat.**Name**
& " [" & swFeat.**GetTypeName** & "]"

    Dim swSketchBend As
SldWorks.SketchedBendFeatureData
    Dim swCustBend As SldWorks.CustomBendAllowance

    Set swSketchBend = swFeat.**GetDefinition**
    Set swCustBend = swSketchBend.**GetCustomBendAllowance**

    Debug.Print "
UseDefaultBendAllowance = " & swSketchBend.**UseDefaultBendAllowance**
    Debug.Print "    UseDefaultBendRadius = " &
swSketchBend.**UseDefaultBendRadius**
    Debug.Print "    BendRadius = " &
swSketchBend.**BendRadius** \* 1000# & " mm"

    Process\_CustomBendAllowance swApp, swModel,
swCustBend

End Sub

Sub Process\_SMMiteredFlange \_
( \_
    swApp As SldWorks.SldWorks, \_
    swModel As SldWorks.ModelDoc2, \_
    swFeat As SldWorks.Feature \_
)

    Debug.Print "  +" & swFeat.**Name**
& " [" & swFeat.**GetTypeName** & "]"

    Dim swMiterFlange As
SldWorks.MiterFlangeFeatureData
    Set swMiterFlange = swFeat.**GetDefinition**

    Debug.Print "
UseDefaultBendAllowance = " & swMiterFlange.**UseDefaultBendAllowance**
    Debug.Print "    UseDefaultBendRadius = " &
swMiterFlange.**UseDefaultBendRadius**
    Debug.Print "    BendRadius = " &
swMiterFlange.**BendRadius** \* 1000# & " mm"

End Sub

Sub Process\_Bends \_
( \_
    swApp As SldWorks.SldWorks, \_
    swModel As SldWorks.ModelDoc2, \_
    swBends As SldWorks.BendsFeatureData \_
)

    Dim swCustBend  As
SldWorks.CustomBendAllowance
    Set swCustBend = swBends.**GetCustomBendAllowance**

    Debug.Print "    BendRadius
= " & swBends.**BendRadius** \* 1000# & " mm"
    Debug.Print "    UseDefaultBendAllowance
= " & swBends.**UseDefaultBendAllowance**
    Debug.Print "    UseDefaultBendRadius
= " & swBends.**UseDefaultBendRadius**

    Process\_CustomBendAllowance swApp, swModel,
swCustBend

End Sub

Sub Process\_ProcessBends \_
( \_
    swApp As SldWorks.SldWorks, \_
    swModel As SldWorks.ModelDoc2, \_
    swFeat As SldWorks.Feature \_
)

    Debug.Print "  +" & swFeat.**Name**
& " [" & swFeat.**GetTypeName** & "]"

    Dim swBends
As SldWorks.BendsFeatureData
    Set swBends = swFeat.**GetDefinition**

    Process\_Bends swApp, swModel, swBends

End Sub

Sub Process\_FlattenBends \_
( \_
    swApp As SldWorks.SldWorks, \_
    swModel As SldWorks.ModelDoc2, \_
    swFeat As SldWorks.Feature \_
)

    Debug.Print "  +" & swFeat.**Name**
& " [" & swFeat.**GetTypeName** & "]"

    Dim swBends
As SldWorks.BendsFeatureData
    Set swBends = swFeat.**GetDefinition**

    Process\_Bends swApp, swModel, swBends

End Sub

Sub Process\_EdgeFlange \_
( \_
    swApp As SldWorks.SldWorks, \_
    swModel As SldWorks.ModelDoc2, \_
    swFeat As SldWorks.Feature \_
)

    Debug.Print "  +" & swFeat.**Name**
& " [" & swFeat.**GetTypeName** & "]"

    Dim swEdgeFlange
As SldWorks.EdgeFlangeFeatureData
    Set swEdgeFlange = swFeat.**GetDefinition**

    Debug.Print "
UseDefaultBendRadius = " & swEdgeFlange.**UseDefaultBendRadius**
    Debug.Print "    BendRadius = " &
swEdgeFlange.**BendRadius** \* 1000# & " mm"

End Sub

Sub Process\_FlatPattern \_
( \_
    swApp As SldWorks.SldWorks, \_
    swModel As SldWorks.ModelDoc2, \_
    swFeat As SldWorks.Feature \_
)

    Debug.Print "  +" & swFeat.**Name**
& " [" & swFeat.**GetTypeName** & "]"

    Dim swFlatPatt
As SldWorks.FlatPatternFeatureData
    Set swFlatPatt = swFeat.**GetDefinition**

    Debug.Print "
Simplify bends? " & swFlatPatt.**SimplifyBends**

End Sub

Sub Process\_Hem \_
( \_
    swApp As SldWorks.SldWorks, \_
    swModel As SldWorks.ModelDoc2, \_
    swFeat As SldWorks.Feature \_
)

    Debug.Print "  +" & swFeat.**Name**
& " [" & swFeat.**GetTypeName** & "]"

    Dim swHem
As SldWorks.HemFeatureData
    Dim swCustBend
As SldWorks.CustomBendAllowance

    Set swHem = swFeat.**GetDefinition**
    Set swCustBend = swHem.**GetCustomBendAllowance**

    Debug.Print "
UseDefaultBendAllowance = " & swHem.**UseDefaultBendAllowance**
    Debug.Print "    Radius = " & swHem.**Radius**
\* 1000# & " mm"

    Process\_CustomBendAllowance swApp, swModel,
swCustBend

End Sub

Sub Process\_Jog \_
( \_
    swApp As SldWorks.SldWorks, \_
    swModel As SldWorks.ModelDoc2, \_
    swFeat As SldWorks.Feature \_
)

    Debug.Print "  +" & swFeat.**Name**
& " [" & swFeat.**GetTypeName** & "]"

    Dim swJog
As SldWorks.JogFeatureData
    Dim swCustBend
As SldWorks.CustomBendAllowance

    Set swJog = swFeat.**GetDefinition**
    Set swCustBend = swJog.**GetCustomBendAllowance**

    Debug.Print "
UseDefaultBendAllowance = " & swJog.**UseDefaultBendAllowance**
    Debug.Print "    UseDefaultBendRadius = " &
swJog.**UseDefaultBendRadius**
    Debug.Print "    BendRadius = " & swJog.**BendRadius**
\* 1000# & " mm"

    Process\_CustomBendAllowance swApp, swModel,
swCustBend

End Sub

Sub Process\_LoftedBend \_
( \_
    swApp As SldWorks.SldWorks, \_
    swModel As SldWorks.ModelDoc2, \_
    swFeat As SldWorks.Feature \_
)

    Debug.Print "  +" & swFeat.**Name**
& " [" & swFeat.**GetTypeName** & "]"

    Dim swLoftBend
As SldWorks.LoftedBendsFeatureData
    Set swLoftBend = swFeat.**GetDefinition**

End Sub

Sub Process\_Rip \_
( \_
    swApp As SldWorks.SldWorks, \_
    swModel As SldWorks.ModelDoc2, \_
    swFeat As SldWorks.Feature \_
)

    Debug.Print "  +" & swFeat.**Name**
& " [" & swFeat.**GetTypeName** & "]"

    Dim swRip
As SldWorks.RipFeatureData
    Set swRip = swFeat.**GetDefinition**

End Sub

Sub Process\_CornerFeat \_
( \_
    swApp As SldWorks.SldWorks, \_
    swModel As SldWorks.ModelDoc2, \_
    swFeat As SldWorks.Feature \_
)

    Debug.Print "  +" & swFeat.**Name**
& " [" & swFeat.**GetTypeName** & "]"

    Dim swCloseCorner
As SldWorks.ClosedCornerFeatureData
    Set swCloseCorner = swFeat.**GetDefinition**

End Sub

Sub Process\_OneBend \_
( \_
    swApp As SldWorks.SldWorks, \_
    swModel As SldWorks.ModelDoc2, \_
    swFeat As SldWorks.Feature \_
)

    Debug.Print "    +" &
swFeat.**Name** & " [" & swFeat.**GetTypeName** & "]"

    Dim swOneBend  As
SldWorks.OneBendFeatureData
    Dim swCustBend As SldWorks.CustomBendAllowance

    Set swOneBend = swFeat.**GetDefinition**
    Set swCustBend = swOneBend.**GetCustomBendAllowance**

    Debug.Print "
UseDefaultBendAllowance = " & swOneBend.**UseDefaultBendAllowance**
    Debug.Print "
UseDefaultBendRadius = " & swOneBend.**UseDefaultBendRadius**

    Process\_CustomBendAllowance swApp, swModel,
swCustBend

End Sub

Sub main()

    Set swApp = Application.**SldWorks**
    Set swModel = swApp.**ActiveDoc**
    Set swSelMgr = swModel.**SelectionManager**
    Set swFeat = swModel.**FirstFeature**

    Debug.Print "File = " & swModel.**GetPathName**

    Do While Not swFeat Is Nothing
        ' Process top-level sheet metal
features
        Select Case swFeat.**GetTypeName**
            Case "SMBaseFlange"

Process\_SMBaseFlange swApp, swModel, swFeat

Case "SheetMetal"

Process\_SheetMetal swApp, swModel, swFeat

Case "SM3dBend"

Process\_SM3dBend swApp, swModel, swFeat

Case "SMMiteredFlange"

Process\_SMMiteredFlange swApp, swModel, swFeat

Case "ProcessBends"

Process\_ProcessBends swApp, swModel, swFeat

Case "FlattenBends"

Process\_FlattenBends swApp, swModel, swFeat

Case "EdgeFlange"

Process\_EdgeFlange swApp, swModel, swFeat

Case "FlatPattern"

Process\_FlatPattern swApp, swModel, swFeat

Case "Hem"

Process\_Hem swApp, swModel, swFeat

Case "Jog"

Process\_Jog swApp, swModel, swFeat

Case "LoftedBend"

Process\_LoftedBend swApp, swModel, swFeat

Case "Rip"

Process\_Rip swApp, swModel, swFeat

Case "CornerFeat"

Process\_CornerFeat swApp, swModel, swFeat

Case Else

' Probably not a sheet metal feature

        End Select

        ' process sheet
metal sub-features
        Set swSubFeat = swFeat.**GetFirstSubFeature**

        Do While Not
swSubFeat Is Nothing
            Select Case
swSubFeat.**GetTypeName**

Case "OneBend"

Process\_OneBend swApp, swModel, swSubFeat

Case Else

' Probably not a sheet metal feature
            End Select

Set swSubFeat = swSubFeat.**GetNextSubFeature**()
        Loop

        Set swFeat =
swFeat.**GetNextFeature**

    Loop

End Sub