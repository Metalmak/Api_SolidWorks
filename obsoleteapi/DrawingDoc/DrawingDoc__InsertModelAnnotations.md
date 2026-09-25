<!-- source: obsoleteapi/DrawingDoc/DrawingDoc__InsertModelAnnotations.htm -->

# DrawingDoc::InsertModelAnnotations

This method is obsolete and has been superseded
by [DrawingDoc::InsertModelAnnotations2](DrawingDoc__InsertModelAnnotations2.htm).

Description

This
method inserts model annotations into this drawing document.

Syntax (OLE Automation)

retval = DrawingDoc.InsertModelAnnotations(
option, allTypes, types, allViews )

| Input: | (long) option | * 0   - All dimensions in the view * 1   - All dimensions of the currently selected component (for assembly drawings) * 2   - All dimensions of the currently selected feature |
| Input: | (BOOL) allTypes | TRUE inserts all types of annotations, FALSE uses the types argument |
| Input: | (long) types | Bitwise OR of annotation types as defined in swInsertAnnotation\_e |
| Input: | (BOOL) allViews | TRUE inserts the annotations in all views in the drawing, FALSE inserts annotations only in the selected view |
| Return: | (BOOL) retval | TRUE if the annotations were added, FALSE if not |

Syntax (COM)

status = DrawingDoc->InsertModelAnnotations(
option )

| Input: | (long) option | * 0   - All dimensions in the view * 1    - All dimensions   of the currently selected component (for assembly drawings) * 2   - All dimensions of the currently selected feature |
| Input: | (VARIANT\_BOOL) allTypes | TRUE inserts all types of annotations, FALSE uses the types argument |
| Input: | (long) types | Bitwise OR of annotation types as defined in swInsertAnnotation\_e |
| Input: | (VARIANT\_BOOL) allViews | TRUE inserts the annotations in all views in the drawing, FALSE inserts annotations only in the selected view |
| Output: | (VARIANT\_BOOL) retval | TRUE if the annotations were added, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks