<!-- source: obsoleteapi/RibFeatureData/RibFeatureData__FlipSide.htm -->

# RibFeatureData::FlipSide

This
property is obsolete and has been superseded by RibFeatureData2::FlipSide.

Description

This property controls whether the material is added to the reverse
side.

Syntax (OLE Automation)

FlipSide= RibFeatureData.FlipSide (VB
Get property)

RibFeatureData.FlipSide= FlipSide (VB
Set property)

FlipSide= RibFeatureData.GetFlipSide
( ) (C++ Get property)

RibFeatureData.SetFlipSide ( FlipSide) (C++
Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (BOOL) FlipSide | TRUE if the material is added to the reverse side |

Syntax (COM)

status = RibFeatureData-> get\_FlipSide(
&FlipSide)

status = RibFeatureData-> put\_FlipSide(
FlipSide)

|  |  |  |
| --- | --- | --- |
| Property: | (VARIANT\_BOOL) FlipSide | TRUE if the material is added to the reverse side |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Changing the value of this property does not affect geometry until Feature::ModifyDefinition
is called.