<!-- source: obsoleteapi/SelectionMgr/SelectionMgr__CreateCallout.htm -->

# SelectionMgr::CreateCallout

This method is obsolete and has been superseded
by SelectionMgr::CreateCallout2.

Description

This method creates a Callout object for a
selection.

Syntax (OLE Automation)

retval = SelectionMgr.CreateCallout ( )

| Output: | (LPCALLOUT) retval | Pointer to the Callout object |

Syntax (COM)

status = SelectionMgr->CreateCallout ( &retval
)

| Output: | (LPCALLOUT) retval | Pointer to the Callout object |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Use this method to create
the callout. Then use SelectionMgr::SetCallout to add the callout to an
already selected object.