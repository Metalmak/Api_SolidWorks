<!-- source: obsoleteapi/RibFeatureData/RibFeatureData__DraftOutward.htm -->

# RibFeatureData::DraftOutward

This
property is obsolete and has been superseded by RibFeatureData2::DraftOutward.

Description

This property controls whether the rib has an associated draft. Additional
draft control can be done with RibFeatureData::DraftAngle and RibFeatureData::EnableDraft.

Syntax (OLE Automation)

DraftOutward= RibFeatureData.DraftOutward (VB
Get property)

RibFeatureData.DraftOutward= DraftOutward (VB
Set property)

DraftOutward= RibFeatureData.GetDraftOutward
( ) (C++ Get property)

RibFeatureData.SetDraftOutward ( DraftOutward) (C++
Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (BOOL) DraftOutward | TRUE if the draft is outward |

Syntax (COM)

status = RibFeatureData-> get\_DraftOutward(
&DraftOutward)

status = RibFeatureData-> put\_DraftOutward(
DraftOutward)

|  |  |  |
| --- | --- | --- |
| Property: | (VARIANT\_BOOL) DraftOutward | TRUE if the draft is outward |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Changing the value of this property does not affect geometry until Feature::ModifyDefinition
is called.