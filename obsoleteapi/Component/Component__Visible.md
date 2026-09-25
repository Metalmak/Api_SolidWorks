<!-- source: obsoleteapi/Component/Component__Visible.htm -->

# Component::Visible

This
property is obsolete and has been superseded by Component2::Visible.

Description

This property gets the visibility state of this component.

Syntax (OLE Automation)

Visible = Component.Visible (VB
Get property)

Visible = Component.GetVisible ( ) (C++
Get property)

|  |  |  |
| --- | --- | --- |
| Property: | (long) Visible | Visibility state of this component instance as defined in swComponentVisibilityState\_e |

Syntax (COM)

status = Component->get\_Visible(
&Visible )

|  |  |  |
| --- | --- | --- |
| Property: | (long) Visible | Visibility state of this component instance as defined in swComponentVisibilityState\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

The functionality of this property is also available with the following
ModelDoc methods:

* ModelDoc2::HideComponent2
* ModelDoc2::ShowComponent2