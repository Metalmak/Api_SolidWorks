<!-- source: obsoleteapi/PartDoc/PartDoc__InsertBends.htm -->

# PartDoc::InsertBends

This method is obsolete and has been superseded
by PartDoc::InsertBends2.

Description

This method creates bends in a thin-feature part.

Syntax (OLE Automation)

retval = PartDoc.InsertBends ( radius, useBendTable,
useKfactor, useBendAllowance, useAutoRelief, offsetRatio )

|  |  |  |
| --- | --- | --- |
| Input: | (double)radius | Radius of the bends |
| Input: | (BSTR)useBendTable | Bend table name (.btl file) |
| Input: | (double) useKfactor | K-Factor ratio or -1 if not used |
| Input: | (double) useBendAllowance | Bend allowance value or -1 if not used |
| Input: | (VARIANT\_BOOL) useAutoRelief | TRUE if auto-relief cuts are to be added |
| Input: | (double) offsetRatio | Distance relief cut extends beyond bend |
| Input: | (VARIANT\_BOOL) retval | TRUE for success, FALSE for failure |

Syntax (COM)

status = PartDoc->InsertBends
( radius, useBendTable, useKfactor, useBendAllowance, useAutoRelief, offsetRatio,
retval )

|  |  |  |
| --- | --- | --- |
| Input: | (double)radius | Radius of the bends |
| Input: | (BSTR)useBendTable | Bend table name (.btl file) |
| Input: | (double) useKfactor | K-Factor ratio or -1 if not used |
| Input: | (double) useBendAllowance | Bend Allowance value or -1 if not used |
| Input: | (VARIANT\_BOOL) useAutoRelief | TRUE if auto-relief cuts are to be added |
| Input: | (double) offsetRatio | Distance relief cut extends beyond bend |
| Input: | (VARIANT\_BOOL) retval | TRUE for success, FALSE for failure |
| Return: | (HRESULT )status | S\_OK if successful |

Remarks

For more information about these arguments, see SolidWorks Help.