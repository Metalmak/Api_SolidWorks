<!-- source: obsoleteapi/AssemblyDoc/AssemblyDoc__EditMate.htm -->

# AssemblyDoc::EditMate

This method is obsolete and has been superseded
by AssemblyDoc::EditMate2.

Description

This method edits the selected assembly component mate relationship.

Syntax (OLE Automation)

void AssemblyDoc.EditMate ( mateType,
align, flip, dist, angle)

| Input: | (long) mateType | Type of mate as defined in swMateType\_e |
| Input: | (long) align | Type of alignment desired as defined in swMateAlign\_e |
| Input: | (VARIANT\_BOOL) flip | TRUE to flip the component, FALSE to not |
| Input: | (double) dist | Distance value used with swMateDISTANCE mate type |
| Input: | (double) angle | Angle value used with swMateANGLE mate type |

Syntax (COM)

status = AssemblyDoc->EditMate (
mateType, align, flip, dist, angle )

| Input: | (long) mateType | Type of mate as defined in swMateType\_e |
| Input: | (long) align | Type of alignment desired as defined in swMateAlign\_e |
| Input: | (VARIANT\_BOOL) flip | TRUE to flip the component, FALSE to not |
| Input: | (double) dist | Distance value used with swMateDISTANCE mate type |
| Input: | (double) angle | Angle value used with swMateANGLE mate type |
| Return: | (HRESULT)status | S\_OK if successful |

Remarks

The first selection should be the two items that are mated (that is,
two faces, edge and face, and so on), and the third selection should be
the mate feature to be edited.

If mateType is swMateDISTANCE or swMateANGLE when the mate is applied
to the closest position that meets the mate condition specified by dist
or angle, then setting flip to TRUE jumps the assembly to the other possible
mate position.