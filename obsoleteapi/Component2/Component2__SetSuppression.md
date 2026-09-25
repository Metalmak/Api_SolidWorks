<!-- source: obsoleteapi/Component2/Component2__SetSuppression.htm -->

# Component2::SetSuppression

This method is obsolete and has been superseded
by Component2::SetSuppression2.

Description

This method sets the suppression state of this component.

Syntax (OLE Automation)

retval = Component2.SetSuppression(
Suppression )

| Input: | (long) Suppression | Suppression state of this component instance as defined in swComponentSuppressionState\_e |
| Return: | (long) retval | One of the values defined in swSuppressionError\_e |

Syntax (COM)

status = Component2->SetSuppression(
Suppression, &retval )

| Input: | (long) Suppression | Suppression state of this component instance as defined in swComponentSuppressionState\_e |
| Output: | (long) retval | One of the values defined in swSuppressionError\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks