<!-- source: obsoleteapi/ModelDoc/ModelDoc__PreTrimSurface.htm -->

# ModelDoc::PreTrimSurface

This
method is obsolete and has been superseded by ModelDoc2::PreTrimSurface.

Description

This method sets the mutual trim option before
trimming a surface.

Syntax (OLE Automation)

void ModelDoc.PreTrimSurface ( bMutualTrimIn)

|  |  |  |
| --- | --- | --- |
| Input: | (BOOL) bMutualTrimIn | TRUE to use the mutual trim option, FALSE otherwise |

Syntax (COM)

status = ModelDoc->PreTrimSurface ( bMutualTrimIn
)

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT\_BOOL) bMutualTrimIn | TRUE to use the mutual trim option, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks