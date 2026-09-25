<!-- source: obsoleteapi/Dimension/Dimension__GetToleranceFontInfo.htm -->

# Dimension::GetToleranceFontInfo

This method is obsolete and has been superseded
by DimensionTolerance::GetFontUseDimension,
DimensionTolerance::GetFontUseScale,
DimensionTolerance::GetFontScale,
and DimensionTolerance::GetFontHeight.

Description

This method gets the tolerance font information for this dimension.

Syntax (OLE Automation)

retval = Dimension.GetToleranceFontInfo
( )

| Return: | (VARIANT) retval | SafeArray of 3 doubles (see Remarks) |

Syntax (COM)

status = Dimension->IGetToleranceFontInfo
( retval )

| Output: | (double\*) retval | Pointer to array of 3 doubles (see Remarks) |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This method returns font information that contains
three values packed into an array of doubles:

[
long useFontScale, double tolScale, double tolHeight
]

| useFontScale | TRUE if the tolerance font size is a scaled value of the dimension font size |
| TolScale | Tolerance font size scale factor based on the dimension font size if useFontScale is TRUE |
| TolHeight | Tolerance height in meters if useFontScale is FALSE |