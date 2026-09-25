<!-- source: obsoleteapi/Component/Component__IsDisplayDataOutOfDate.htm -->

# Component::IsDisplayDataOutOfDate

This
method is obsolete and has been superseded by Component2::IsDisplayDataOutOfDate.

Description

This method provides the status of the display
data for this component.

Syntax (OLE Automation)

retval = Component.IsDisplayDataOutOfDate ( )

| Return: | (long) retval | Rebuild state of the components as defined in swOutOfDateStatus\_e |

Syntax (COM)

status = Component->IsDisplayDataOutOfDate ( &retval
)

| Output: | (long) retval | Rebuild state of the components as defined in  swOutOfDateStatus\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks