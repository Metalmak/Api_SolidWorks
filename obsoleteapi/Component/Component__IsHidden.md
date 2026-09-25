<!-- source: obsoleteapi/Component/Component__IsHidden.htm -->

# Component::IsHidden

This method is obsolete and has been superseded by Component2::IsHidden.

Description

This method determines if this component is hidden or suppressed.

Syntax (OLE Automation)

retval
= Component.IsHidden ( considerSuppressed )

| Input: | (BOOL) considerSuppressed | Controls whether suppressed components are considered hidden |
| Return: | (BOOL) retval | TRUE or FALSE (see Remarks) |

Syntax (COM)

status
= Component->IsHidden ( considerSuppressed, &retval )

| Input: | (VARIANT\_BOOL) considerSuppressed | Controls whether suppressed components are considered hidden |
| Output: | (VARIANT\_BOOL) retval | TRUE or FALSE (see Remarks) |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks

The state of this component can vary based on the active configuration.

| ConsiderSuppressed | Component | Component | IsHidden |
| True | Hidden | Unsuppressed | True |
| True | Hidden | Suppressed | True |
| True | Shown | Unsuppressed | True |
| True | Shown | Suppressed | False |
| False | Hidden | Unsuppressed | True |
| False | Hidden | Suppressed | True |
| False | Shown | Unsuppressed | False |
| False | Shown | Suppressed | False |

NOTE:
For lightweight components, Componet::IsHidden returns TRUE if considerSuppressed
is TRUE.