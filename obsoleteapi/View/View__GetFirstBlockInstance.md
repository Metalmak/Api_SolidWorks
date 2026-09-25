<!-- source: obsoleteapi/View/View__GetFirstBlockInstance.htm -->

# View::GetFirstBlockInstance

This method is obsolete and was not superseded.

Description

This method gets the first block instance in
this view.

Syntax (OLE Automation)

retval = View.GetFirstBlockInstance ( )

|  |  |  |
| --- | --- | --- |
| Output: | (LPBLOCKINSTANCE) retval | Pointer to the first BlockInstance object |

Syntax (COM)

status = View->GetFirstBlockInstance ( &retval
)

|  |  |  |
| --- | --- | --- |
| Output: | (LPBLOCKINSTANCE) retval | Pointer to the first BlockInstance object |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

The sheet must be visible.
See Sheet::SheetFormatVisible.