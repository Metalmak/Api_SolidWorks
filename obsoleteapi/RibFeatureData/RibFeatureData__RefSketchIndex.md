<!-- source: obsoleteapi/RibFeatureData/RibFeatureData__RefSketchIndex.htm -->

# RibFeatureData::RefSketchIndex

This
property is obsolete and has been superseded by RibFeatureData2::RefSketchIndex.

Description

This property specifies which sketch segment defines the draft direction
of the rib feature.

Syntax (OLE Automation)

Index= RibFeatureData.RefSketchIndex (VB
Get property)

RibFeatureData.RefSketchIndex= Index (VB
Set property)

Index= RibFeatureData.GetRefSketchIndex
( ) (C++ Get property)

RibFeatureData.SetRefSketchIndex (
Index ) (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (int) Index | Index of the sketch segment |

Syntax (COM)

status = RibFeatureData-> get\_RefSketchIndex(
&Index)

status = RibFeatureData-> put\_RefSketchIndex(
Index)

|  |  |  |
| --- | --- | --- |
| Property: | (double) Thickness | Index of the sketch segment |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks