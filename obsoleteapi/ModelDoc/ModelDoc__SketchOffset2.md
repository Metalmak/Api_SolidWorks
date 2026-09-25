<!-- source: obsoleteapi/ModelDoc/ModelDoc__SketchOffset2.htm -->

# ModelDoc::SketchOffset2

This
method is obsolete and has been superseded by ModelDoc2::SketchOffset2.

Description

This method offsets sketch segments.

Syntax (OLE Automation)

retval = ModelDoc.SketchOffset2 ( offset, bothDirections,
chain )

|  |  |  |
| --- | --- | --- |
| Input: | (double) offset | Desired offset value; negative value will offset in opposite direction |
| Input: | (BOOL) bothDirections | TRUE to offset in both directions |
| Input: | (BOOL) chain | TRUE if you want entire chain of entities offset, FALSE if you want only selected sketch entities offset |
| Return: | (BOOL) retval | TRUE if the offset was successful |

Syntax (COM)

status = ModelDoc->SketchOffset2 ( offset, bothDirections,
chain, &retval )

|  |  |  |
| --- | --- | --- |
| Input: | (double) offset | Desired offset value; negative value will offset in opposite direction |
| Input: | (VARIANT\_BOOL) bothDirections | TRUE to offset in both directions |
| Input: | (VARIANT\_BOOL) chain | TRUE if you want entire chain of entities offset, FALSE if you want only selected sketch entities offset |
| Output: | (VARIANT\_BOOL) retval | TRUE if the offset was successful |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Specifying TRUE to the chain argument offsets the
selected entity and any other entities that belong to the same contour
or chain; for example, contiguous geometric entities like edges.