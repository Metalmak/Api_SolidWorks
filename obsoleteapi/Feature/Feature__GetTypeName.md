<!-- source: obsoleteapi/Feature/Feature__GetTypeName.htm -->

# Feature::GetTypeName

This method is obsolete and has been superseded
by Feature::GetTypeName2.

Description

This
method gets the type of feature.

Syntax (OLE Automation)

retval = Feature.GetTypeName ()

| Return: | (BSTR) retval | Feature type as defined in BodyFeatures\_e |

Syntax (COM)

status = Feature->GetTypeName (
&retval )

| Output: | (BSTR) retval | Feature type as defined in BodyFeatures\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

For example, if this feature is a plane, then
this method returns swTnRefPlane, which is equivalent to the string value
"RefPlane".