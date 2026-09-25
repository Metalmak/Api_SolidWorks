<!-- source: obsoleteapi/ModelDoc/ModelDoc__GetInferenceMode.htm -->

# ModelDoc::GetInferenceMode

This
method is obsolete and has been superseded byModelDoc2::GetInferenceMode.

Description

This method determines whether the sketch inference
mode for this ModelDoc has been turned off or not. This affects sketch
entity snapping, or inferring constraints to other geometry, during creation.

Syntax (OLE Automation)

inferenceMode = ModelDoc.GetInferenceMode ( )

|  |  |  |
| --- | --- | --- |
| Return: | (BOOL) inferenceMode | TRUE if sketch inference mode is enabled, FALSE if it is  disabled |

Syntax (COM)

status = ModelDoc->GetInferenceMode ( &inferenceMode
)

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT\_BOOL) inferenceMode | TRUE if sketch inference mode is enabled, FALSE if it is disabled |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks