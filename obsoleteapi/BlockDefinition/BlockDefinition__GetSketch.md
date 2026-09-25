<!-- source: obsoleteapi/BlockDefinition/BlockDefinition__GetSketch.htm -->

# BlockDefinition::GetSketch

This method is obsolete and has been superseded
by SketchBlockDefinition::GetSketch.

Description

This method gets the sketch for this block
definition.

Syntax (OLE Automation)

retval = BlockDefinition.GetSketch ( )

#

|  |  |  |
| --- | --- | --- |
| Output: | (LPSKETCH) retval | Pointer to the Sketch object |

#

Syntax (COM)

status = BlockDefinition->GetSketch ( &retval
)

|  |  |  |
| --- | --- | --- |
| Output: | (LPSKETCH) retval | Pointer to the Sketch object |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks

You cannot modify the returned
sketch. It is read-only.