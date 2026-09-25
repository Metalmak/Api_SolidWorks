<!-- source: obsoleteapi/Dimension/Dimension__GetToleranceType.htm -->

# Dimension::GetToleranceType

This method is obsolete and has been superseded
by DimensionTolerance::Type.

Description

This
method gets the type of tolerance of the dimension.

Syntax (OLE Automation)

retval = Dimension.GetToleranceType
( )

|  |  |  |
| --- | --- | --- |
| Return: | (long) retval | Tolerance type as defined in swTolType\_e |

Syntax (COM)

status = Dimension->GetToleranceType
( &retval )

|  |  |  |
| --- | --- | --- |
| Output: | (long) retval | Tolerance type as defined in swTolType\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks