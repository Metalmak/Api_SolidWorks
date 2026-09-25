<!-- source: obsoleteapi/ModelDoc/ModelDoc__InsertScale.htm -->

# ModelDoc::InsertScale

This
method is obsolete and has been superseded by [ModelDoc2::InsertScale](../ModelDoc2/ModelDoc2__InsertScale.htm).

Description

This method applies a scaling factor to the
model.

Syntax (OLE Automation)

void ModelDoc.InsertScale (
scaleFactor\_x, scaleFactor\_y, scaleFactor\_z, isUniform, scaleType )

|  |  |  |
| --- | --- | --- |
| Input: | (double) scaleFactor\_x | X component of the scale factor |
| Input: | (double) scaleFactor\_y | Y component of the scale factor |
| Input: | (double) scaleFactor\_z | Z component of the scale factor |
| Input: | (BOOL) isUniform | TRUE if the scaling should be uniform, FALSE otherwise. |
| Input: | (int) scaleType | Type of scale as defined in swScaleType\_e |

Syntax (COM)

status = ModelDoc->InsertScale ( scaleFactor\_x,
scaleFactor\_y, scaleFactor\_z, isUniform, scaleType )

|  |  |  |
| --- | --- | --- |
| Input: | (double) scaleFactor\_x | X component of the scale factor |
| Input: | (double) scaleFactor\_y | Y component of the scale factor |
| Input: | (double) scaleFactor\_z | Z component of the scale factor |
| Input: | (BOOL) isUniform | TRUE if the scaling should be uniform, FALSE otherwise |
| Input: | (int) scaleType | Type of scale as defined in swScaleType\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

If isUniform is TRUE, then scaleFactor\_x  is
used as the uniform scaling factor. If isUniform is FALSE, then all three
scaling factors are used.