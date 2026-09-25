<!-- source: obsoleteapi/View/View__GetDisplayTangentEdges.htm -->

# View::GetDisplayTangentEdges

This
method is obsolete and has been superseded by View::GetDisplayTangentEdges2.

Description

This method determines the current tangent edge display mode of the
drawing view.

NOTE: Tangent edges are the
transition line between, for example, a blend and a face.

Syntax (OLE Automation)

retval = View.GetDisplayTangentEdges
()

|  |  |  |
| --- | --- | --- |
| Return: | (BOOL) retval | TRUE if tangent edges are currently being shown, FALSE otherwise |

Syntax (COM)

status = View->GetDisplayTangentEdges
( &retval )

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if tangent edges are currently being shown, FALSE otherwise |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks