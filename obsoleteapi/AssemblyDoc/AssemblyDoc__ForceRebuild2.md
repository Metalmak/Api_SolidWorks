<!-- source: obsoleteapi/AssemblyDoc/AssemblyDoc__ForceRebuild2.htm -->

# AssemblyDoc::ForceRebuild2

This
method is obsolete and has been superseded by ModelDoc2::ForceRebuild3.

Description

This method forces a rebuild of the assembly.

Syntax (OLE Automation)

void AssemblyDoc.ForceRebuild2 ( topOnly
)

| Input: | (BOOL) topOnly | TRUE if you want  to rebuild the top level of assembly only; FALSE if you want to rebuild the top level and all subassemblies |

Syntax (COM)

status = AssemblyDoc->ForceRebuild2 ( topOnly
)

| Input: | (VARIANT\_BOOL) topOnly | TRUE if you want to rebuild the top level of assembly only; FALSE if you want to rebuild the top level and all subassemblies |
| Return: | (HRESULT) status | S\_OK if successful; S\_FALSE otherwise |

Remarks

This command rebuilds the entire model, whether
or not it needs to be rebuilt. This operation can be very time consuming.
Use the topLevelOnly argument to enhance performance.