<!-- source: obsoleteapi/Component/Component__IsFixed.htm -->

# Component::IsFixed

This
method is obsolete and has been superseded by Component2::IsFixed.

Description

This method determines if the component is fixed or floating.

Syntax (OLE Automation)

retval
= Component.IsFixed ()

|  |  |  |
| --- | --- | --- |
| Return: | (BOOL) retval | TRUE if this component is fixed, FALSE if this component is floating |

Syntax (COM)

status = Component->IsFixed ( &retval
)

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if this component is fixed, FALSE if this component is floating |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks