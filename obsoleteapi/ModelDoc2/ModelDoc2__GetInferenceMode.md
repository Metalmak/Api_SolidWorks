<!-- source: obsoleteapi/ModelDoc2/ModelDoc2__GetInferenceMode.htm -->

# ModelDoc2::GetInferenceMode

This
method is obsolete and has been superseded by SketchManager::InferenceMode.

Description

This method determines whether the sketch inference
mode is on or off. This affects sketch-entity snapping or inferring constraints
to other geometry during creation.

Syntax (OLE Automation)

inferenceMode = ModelDoc2.GetInferenceMode ( )

|  |  |  |
| --- | --- | --- |
| Return: | (BOOL) inferenceMode | TRUE if sketch inference mode is enabled, FALSE if disabled |

Syntax (COM)

status = ModelDoc2->GetInferenceMode ( &inferenceMode
)

| Input: | (VARIANT\_BOOL) inferenceMode | TRUE if sketch inference mode is enabled, FALSE if disabled. |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks