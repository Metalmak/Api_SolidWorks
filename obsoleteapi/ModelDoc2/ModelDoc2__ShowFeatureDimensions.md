<!-- source: obsoleteapi/ModelDoc2/ModelDoc2__ShowFeatureDimensions.htm -->

# ModelDoc2::ShowFeatureDimensions

This method is obsolete and has been superseded.
Use ModelDoc2::GetUserPreferenceToggle
or ModelDoc2::SetUserPreferenceToggle
and swDisplayFeatureDimensions.

Description

This method displays all of the dimensions
of the selected feature.

Syntax (OLE Automation)

void ModelDoc2.ShowFeatureDimensions ( )

Syntax (COM)

status = ModelDoc2->ShowFeatureDimensions ( )

| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This method supports part and assembly documents;
it does not affect drawing documents.