<!-- source: obsoleteapi/ModelDoc/ModelDoc__GetBlockingState.htm -->

# ModelDoc::GetBlockingState

This
method is obsolete and has been superseded by ModelDoc2::GetBlockingState.

Description

This method gets the current value of the SolidWorks
blocking state within the

range of values accessible by ModelDoc2::SetBlockingState,
 for example,
swFullBlock,

swModifyBlock, or swNoBlock.

Syntax (OLE Automation)

retval = ModelDoc.GetBlockingState ( )

|  |  |  |
| --- | --- | --- |
| Return: | (long) retval | Value as defined in swBlockingStates\_e |

Syntax (COM)

status = ModelDoc->GetBlockingState ( &retval
)

|  |  |  |
| --- | --- | --- |
| Output: | (long) retval | Value as defined in swBlockingStates\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks