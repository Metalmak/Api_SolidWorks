<!-- source: obsoleteapi/Annotation/Annotation__GetLeader.htm -->

# Annotation::GetLeader

This method is obsolete and has been superseded
by Annotation::GetLeaderStyle.

Description

This method gets the leader display setting
for this annotation.

Syntax (OLE Automation)

retval = Annotation.GetLeader ( )

| Return: | (BOOL) retval | TRUE if leader display is enabled for this annotation, FALSE if leader display is disabled for this annotation |

Syntax (COM)

status = Annotation->GetLeader ( &retval )

| Output: | (VARIANT\_BOOL) retval | TRUE if leader display is enabled for this annotation, FALSE if leader display is disabled for this annotation |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks

Use Annotation::SetLeader2 to enable or disable
leader display.

NOTE: Dimension
annotations do not have leaders. Therefore, this method always returns
FALSE for dimension annotations.