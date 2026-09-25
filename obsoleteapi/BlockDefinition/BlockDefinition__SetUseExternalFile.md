<!-- source: obsoleteapi/BlockDefinition/BlockDefinition__SetUseExternalFile.htm -->

# BlockDefinition::SetUseExternalFile

This method is obsolete and has been superseded
by SketchBlockDefinition::LinkToFile.

Description

This method sets whether or not this block
definition is maintaining a link to an external file.

Syntax (OLE Automation)

retval = BlockDefinition.SetUseExternalFile ( UseFile
)

| Input: | (VARIANT\_BOOL) UseFile | TRUE enables the link between the block definition and the external file, FALSE disables the link |
| Output: | (long) retval | Status of the external file link as defined in swBlockDefinitionExtFileStatus\_e |

Syntax (COM)

status = BlockDefinition->SetUseExternalFile (
UseFile, &retval )

| Input: | (VARIANT\_BOOL) UseFile | TRUE enables the link between the block definition and the external file, FALSE disables the link |
| Output: | (long) retval | Status of the external file link as defined in swBlockDefinitionExtFileStatus\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

To determine if this block
definition is currently linked to an external file, use BlockDefinition::GetUseExternalFile.
To get the name of the external file, use BlockDefinition::GetExternalFileName.