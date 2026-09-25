<!-- source: obsoleteapi/RibFeatureData/RibFeatureData__ReverseThicknessDir.htm -->

# RibFeatureData::ReverseThicknessDir

This
property is obsolete and has been superseded by RibFeatureData2::ReverseThicknessDir.

Description

If a rib is single-sided, then this property specifies whether the extrusion
is on the reverse side.

Syntax (OLE Automation)

Reverse= RibFeatureData.ReverseThicknessDir (VB
Get property)

RibFeatureData.ReverseThicknessDir=
Reverse (VB Set property)

Reverse= RibFeatureData.GetReverseThicknessDir
( ) (C++ Get property)

RibFeatureData.SetReverseThicknessDir
( Reverse) (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (BOOL) Reverse | TRUE if the rib is extruded on the reverse side |

Syntax (COM)

status = RibFeatureData-> get\_ReverseThicknessDir(
&Reverse)

status = RibFeatureData-> put\_ReverseThicknessDir(
Reverse)

|  |  |  |
| --- | --- | --- |
| Property: | (VARIANT\_BOOL) Reverse | TRUE if the rib is extruded on the reverse side |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks

Changing the value of this property does not affect geometry until Feature::ModifyDefinition
is called.