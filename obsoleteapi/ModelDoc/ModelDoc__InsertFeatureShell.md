<!-- source: obsoleteapi/ModelDoc/ModelDoc__InsertFeatureShell.htm -->

# ModelDoc::InsertFeatureShell

This
method is obsolete and has been superseded by ModelDoc2::InsertFeatureShell.

Description

This method creates a shell feature.

Syntax (OLE Automation)

void ModelDoc.InsertFeatureShell (
thickness, outward)

|  |  |  |
| --- | --- | --- |
| Input: | (double) thickness | Shell thickness in meters |
| Input: | (BOOL) outward | TRUE for outside, FALSE for inside |

Syntax (COM)

status = ModelDoc->InsertFeatureShell
( thickness, outward )

|  |  |  |
| --- | --- | --- |
| Input: | (double) thickness | Shell thickness in meters |
| Input: | (VARIANT\_BOOL) outward | TRUE for outside, FALSE for inside |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

This method is the same as interactively creating a planar surface by
selecting Insert,
Features, Shell.

See the SolidWorks Help for more information about what
entities are valid for selection.

Make the selections using ModelDoc::SelectByID before calling this method.

To make a multi-thickness shell, you can make additional calls to ModelDoc::InsertFeatureShellAddThickness
after making the selections and before calling this method.