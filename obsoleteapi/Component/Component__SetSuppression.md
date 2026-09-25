<!-- source: obsoleteapi/Component/Component__SetSuppression.htm -->

# Component::SetSuppression

This
method is obsolete and has been superseded by [Component2::SetSuppression](../Component2/Component2__SetSuppression.htm).

Description

This method controls the suppression state of this component.

Syntax (OLE Automation)

retval = Component.SetSuppression(
Suppression )

| Input: | (long) Suppression | Suppression state of this component instance as defined in swComponentSuppressionState\_e |
| Return: | (long) retval | Error code as defined in swSuppressionError\_e |

Syntax (COM)

status = Component->SetSuppression(
Suppression, &retval )

| Input: | (long) Suppression | Suppression state of this component instance as defined in swComponentSuppressionState\_e |
| Output: | (long) retval | Error code as defined in swSuppressionError\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

You cannot set a component to lightweight (for example, Suppression
= swComponentLightweight is not valid).