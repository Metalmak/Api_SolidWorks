<!-- source: obsoleteapi/DisplayDimension/Dimension__GetToleranceFitValues.htm -->

# Dimension::GetToleranceFitValues

This method is obsolete and has been superseded
by DimensionTolerance::GetHoleFitValue
and DimensionTolerance::GetShaftFitValue.

Description

This
method gets the tolerance values for fit tolerances.

Syntax (OLE Automation)

retval
= Dimension.GetToleranceFitValues ( )

| Return: | (BSTR) retval | String containing the two fit values separated by a comma |

Syntax (COM)

status = Dimension->GetToleranceFitValues
( &retval )

| Output: | (BSTR) retval | String containing the two fit values separated by a comma |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks