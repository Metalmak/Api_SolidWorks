<!-- source: obsoleteapi/BlockDefinition/BlockDefinition__SetExternalFileName.htm -->

# BlockDefinition::SetExternalFileName

This method is obsolete and has been superseded
by SketchBlockDefinition::FileName.

Description

This method sets the name of the file that
the block definition references.

Syntax (OLE Automation)

retval = BlockDefinition.SetExternalFileName ( Filename
)

| Input: | (BSTR) Filename | Name of the file |
| Output: | (long) retval | Status of the external file link as defined in swBlockDefinitionExtFileStatus\_e |

Syntax (COM)

status = BlockDefinition->SetExternalFileName
( Filename, &retval )

| Input: | (BSTR) Filename | Name of the file |
| Output: | (long) retval | Status of the external file link as defined in swBlockDefinitionExtFileStatus\_e |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

To determine if this block
definition is currently linked to an external file, use BlockDefinition::GetUseExternalFile.
To get the name of the external file, use BlockDefinition::GetExternalFileName.