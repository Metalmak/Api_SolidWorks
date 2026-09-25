<!-- source: obsoleteapi/ExtrudeFeatureData/ExtrudeFeatureData__FlipSideToCut.htm -->

# ExtrudeFeatureData::FlipSideToCut

This
property is obsolete and has been superseded by ExtrudeFeatureData2::FlipToSideCut.

Description

This property gets or sets whether to flip
the side to cut.

Syntax (OLE Automation)

flip = ExtrudeFeatureData.FlipSideToCut  (VB
Get property)

ExtrudeFeatureData.FlipSideToCut = flip  (VB Set property)

flip
= ExtrudeFeatureData.GetFlipSideToCut ( ) (C++ Get property)

ExtrudeFeatureData.SetFlipSideToCut (flip)  (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (BOOL) flip | TRUE flips the side to cut, FALSE does not |

Syntax (COM)

status = ExtrudeFeatureData->get\_ FlipSideToCut
( &flip)

status = ExtrudeFeatureData->put\_ FlipSideToCut
(flip)

|  |  |  |
| --- | --- | --- |
| Property: | (VARIANT\_BOOL) flip | TRUE flips the side to cut, FALSE does not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This property is relevant only for cut features.