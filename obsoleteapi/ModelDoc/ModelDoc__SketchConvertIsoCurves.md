<!-- source: obsoleteapi/ModelDoc/ModelDoc__SketchConvertIsoCurves.htm -->

# ModelDoc::SketchConvertIsoCurves

This method is obsolete
and has been superseded by ModelDoc2::SketchConvertIsoCurves.

Description

This method converts an ISO-parametric curve
or curves on a selected surface into a sketch entity.

Syntax (OLE Automation)

void ModelDoc.SketchConvertIsoCurves ( percentRatio,
vORuDir, doConstrain, skipHoles)

|  |  |  |
| --- | --- | --- |
| Input: | (double) percentRatio | Value for percent ratio |
| Input: | (BOOL) vORuDir | TRUE for V direction, FALSE for U direction |
| Input: | (BOOL) doConstrain | TRUE if you want to constrain these new sketch entities, FALSE otherwise |
| Input | (BOOL) skipHoles | TRUE if you want to skip the holes in this surface, FALSE otherwise |

Syntax (COM)

status = ModelDoc->SketchConvertIsoCurves ( percentRatio,
vORuDir, doConstrain)

|  |  |  |
| --- | --- | --- |
| Input: | (double) percentRatio | Value for percent ratio |
| Input: | (VARIANT\_BOOL) vORuDir | TRUE for V direction, FASLE for U direction |
| Input: | (VARIANT\_BOOL) doConstrain | TRUE if you want to constrain these new sketch entities, FALSE otherwise |
| Input | (VARIANT\_BOOL) skipHoles | TRUE if you want to skip the holes in this surface, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks