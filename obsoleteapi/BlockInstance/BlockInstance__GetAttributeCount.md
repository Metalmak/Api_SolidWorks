<!-- source: obsoleteapi/BlockInstance/BlockInstance__GetAttributeCount.htm -->

# BlockInstance::GetAttributeCount

This method is obsolete and has been superseded
by SketchBlockInstance::GetAttributeCount.

Description

This method gets the number of attributes for
the block.

Syntax (OLE Automation)

retval = BlockInstance.GetAttributeCount ( )

#

|  |  |  |
| --- | --- | --- |
| Output: | (long) retval | Number of attributes for the block |

#

Syntax (COM)

status = BlockInstance->GetAttributeCount ( &retval
)

|  |  |  |
| --- | --- | --- |
| Output: | (long) retval | Number of attributes for the block |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks