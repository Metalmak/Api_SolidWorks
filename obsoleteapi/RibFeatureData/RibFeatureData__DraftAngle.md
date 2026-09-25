<!-- source: obsoleteapi/RibFeatureData/RibFeatureData__DraftAngle.htm -->

# RibFeatureData::DraftAngle

This
property is obsolete and has been superseded by RibFeatureData2::DraftAngle.

Description

This property controls the draft angle for the rib. Additional draft
control can be done with RibFeatureData::EnableDraft and RibFeatureData::DraftOutward.

Syntax (OLE Automation)

DraftAngle= RibFeatureData.DraftAngle (VB
Get property)

RibFeatureData.DraftAngle= DraftAngle (VB
Set property)

DraftAngle= RibFeatureData.GetDraftAngle
( ) (C++ Get property)

RibFeatureData.SetDraftAngle ( DraftAngle) (C++
Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (double) DraftAngle | Angle for the draft |

Syntax (COM)

status = RibFeatureData-> get\_DraftAngle(
&DraftAngle)

status = RibFeatureData-> put\_DraftAngle(
DraftAngle)

|  |  |  |
| --- | --- | --- |
| Property: | (double) DraftAngle | Angle for the draft |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Changing the value of this property does not affect geometry until Feature::ModifyDefinition
is called.