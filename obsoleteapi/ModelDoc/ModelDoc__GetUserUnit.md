<!-- source: obsoleteapi/ModelDoc/ModelDoc__GetUserUnit.htm -->

# ModelDoc::IGetUserUnit

This
method is obsolete and has been superseded by ModelDoc2::GetUserUnit.

Description

This method will return the user units.

Syntax (OLE Automation)

retval = ModelDoc.GetUserUnit ( UnitType )

|  |  |  |  |
| --- | --- | --- | --- |
| Input: | (long) UnitType | User unit type as defined in swUserUnitsType\_e |  |
| Output: | (LPUSERUNIT) retval | Pointer to the user unit object |  |

Syntax (COM)

status = ModelDoc->IGetUserUnit ( UnitType, &retval
)

|  |  |  |  |
| --- | --- | --- | --- |
| Input: | (long) UnitType | User unit type as defined in swUserUnitsType\_e |  |
| Output: | (LPUSERUNIT) retval | Pointer to the user unit object |  |
| Return: | (HRESULT) status | S\_OK if successful | S\_OK if successful |

Remarks