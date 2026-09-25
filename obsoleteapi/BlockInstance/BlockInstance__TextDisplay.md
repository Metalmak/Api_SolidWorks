<!-- source: obsoleteapi/BlockInstance/BlockInstance__TextDisplay.htm -->

# BlockInstance::TextDisplay

This property is obsolete and has been superseded
by SketchBlockInstance::TextDisplay.

Description

This property gets and sets
whether to display text for the block.

Syntax (OLE Automation)

propval = BlockInstance.TextDisplay (VB Get property)

BlockInstance.TextDisplay = propval (VB Set property)

propval = BlockInstance.GetTextDisplay ( ) (C++ Get
property)

BlockInstance.SetTextDisplay ( propval ) (C++ Set
property)

#

|  |  |  |
| --- | --- | --- |
| Property: | (long) propval | Long as defined in swBlockInstanceTextDisplay\_e |

#

Syntax (COM)

status = BlockInstance->get\_TextDisplay ( &propval
)

status = BlockInstance->put\_TextDisplay ( propval
)

|  |  |  |
| --- | --- | --- |
| Property: | (long) propval | Long as defined in swBlockInstanceTextDisplay\_e |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks