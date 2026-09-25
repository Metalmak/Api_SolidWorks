<!-- source: obsoleteapi/ModelDoc/ModelDoc__PostTrimSurface.htm -->

# ModelDoc::PostTrimSurface

This
method is obsolete and has been superseded by ModelDoc2::PostTrimSurface.

Description

This method sets the option for the trim surface
post-process type.

Syntax (OLE Automation)

void ModelDoc.PostTrimSurface ( bSewSurfaceIn)

|  |  |  |
| --- | --- | --- |
| Input: | (BOOL) bSewSurfaceIn | TRUE if you want to use the sew surface in option, FALSE otherwise |

Syntax (COM)

status = ModelDoc->PostTrimSurface ( bSewSurfaceIn
)

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT\_BOOL) bSewSurfaceIn | TRUE if you want to use the sew surface in option, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks