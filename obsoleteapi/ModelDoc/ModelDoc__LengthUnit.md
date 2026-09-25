<!-- source: obsoleteapi/ModelDoc/ModelDoc__LengthUnit.htm -->

# ModelDoc::LengthUnit

This
property is obsolete and has been superseded by ModelDoc2::LengthUnit.

Description

This property gets and sets the length unit. This property will get
and set the same LengthUnit value used by ModelDoc::GetUnits and ModelDoc::SetUnits.

Syntax (OLE Automation)

LengthUnit = ModelDoc.LengthUnit (VB
Get property)

ModelDoc.LengthUnit = LengthUnit (VB
Set property)

LengthUnit = ModelDoc.GetLengthUnit
( ) (C++ Get property)

ModelDoc.SetLengthUnit ( LengthUnit
) (C++ Set property)

|  |  |  |
| --- | --- | --- |
| Property: | (long) LengthUnit | Units as defined in swLengthUnit\_e |

Syntax (Com)

status = ModelDoc->get\_LengthUnit(
&LengthUnit )

status = ModelDoc->put\_LengthUnit(
LengthUnit )

|  |  |  |
| --- | --- | --- |
| Property: | (long) LengthUnit | Units as defined in swLengthUnit\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks