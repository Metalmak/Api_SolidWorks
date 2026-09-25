<!-- source: obsoleteapi/ModelDoc2/ModelDoc2__HideFeatureDimensions.htm -->

# ModelDoc2::HideFeatureDimensions

This method is obsolete and has been superseded.
Use ModelDoc2::GetUserPreferenceToggle
or ModelDoc2::SetUserPreferenceToggle
and swDisplayFeatureDimensions.

Description

This method causes all of the dimensions of
the selected feature to be hidden in this document.

Syntax (OLE Automation)

void ModelDoc2.HideFeatureDimensions ( )

Syntax (COM)

status = ModelDoc2->HideFeatureDimensions ( )

| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This method only applies to part and assembly documents;
it does not affect a drawing document.