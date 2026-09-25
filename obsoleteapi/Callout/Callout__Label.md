<!-- source: obsoleteapi/Callout/Callout__Label.htm -->

# Callout::Label

This method is obsolete and has been superseded
by Callout::Label2.

Description

This property gets or sets the text for this
callout.

Syntax (OLE Automation)

retval = Callout.Label (VB Get property)

Callout.Label = retval (VB Set property)

retval = Callout.GetLabel ( ) (C++ Get property)

Callout.SetLabel ( retval ) (C++ Set property)

| Property: | (BSTR) retval | Callout text |

#

Syntax (COM)

status = Callout->get\_Label ( &retval )

status = Callout->put\_Label ( retval )

| Property: | (BSTR) retval | Callout text |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

The label cannot
be:

* an
  empty string.
* edited
  after it is displayed.