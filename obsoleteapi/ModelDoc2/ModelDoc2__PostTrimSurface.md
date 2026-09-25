<!-- source: obsoleteapi/ModelDoc2/ModelDoc2__PostTrimSurface.htm -->

# ModelDoc2::PostTrimSurface

This
method is obsolete and has been superseded by FeatureManager::PostTrimSurface.

Description

This method sets the Trim
tool option for the surface post-processing type.

Syntax (OLE Automation)

void ModelDoc2.PostTrimSurface ( bSewSurfaceIn)

|  |  |  |
| --- | --- | --- |
| Input: | (BOOL) bSewSurfaceIn | TRUE to set Trim tool option, FALSE otherwise |

Syntax (COM)

status = ModelDoc2->PostTrimSurface ( bSewSurfaceIn
)

| Input: | (VARIANT\_BOOL) bSewSurfaceIn | TRUE to Trim tool option, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

See SolidWorks Help for details about this option.