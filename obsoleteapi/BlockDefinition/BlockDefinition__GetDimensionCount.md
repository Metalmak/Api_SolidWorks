<!-- source: obsoleteapi/BlockDefinition/BlockDefinition__GetDimensionCount.htm -->

# BlockDefinition::GetDimensionCount

This method is obsolete and has been superseded
by SketchBlockDefinition::GetDisplayDimensionCount.

Description

This method gets the number of displayed dimensions
for the block definition.

Syntax (OLE Automation)

retval = BlockDefinition.GetDimensionCount ( )

#

|  |  |  |
| --- | --- | --- |
| Output: | (long) retval | Number of displayed dimensions |

#

Syntax (COM)

status = BlockDefinition->GetDimensionCount (
&retval )

|  |  |  |
| --- | --- | --- |
| Output: | (long) retval | Number of displayed dimensions |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks