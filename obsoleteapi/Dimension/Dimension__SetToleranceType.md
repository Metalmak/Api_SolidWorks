<!-- source: obsoleteapi/Dimension/Dimension__SetToleranceType.htm -->

# Dimension::SetToleranceType

This
method is obsolete and has been superseded by DimensionTolerance::Type.

Description

This
method sets the tolerance type of the dimension.

Syntax (OLE Automation)

retval
= Dimension.SetToleranceType ( newType )

| Input: | (long) newType | Tolerance type as defined in swTolType\_e |
| Return: | (BOOL) retval | TRUE if the tolerance type was set successfully, FALSE if it was not |

Syntax (COM)

status = Dimension->SetToleranceType
( newType, &retval )

| Input: | (long) newType | Tolerance type as defined in swTolType\_e |
| Output: | (VARIANT\_BOOL) retval | TRUE if the tolerance type was set successfully, FALSE if it was not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks