<!-- source: obsoleteapi/BomFeature/BomFeature__FollowAssemblyOrder.htm -->

# BomFeature::FollowAssemblyOrder

This method is obsolete and has been superseded
by BomFeature::FollowAssemblyOrder2.

Description

This method sets the order
of the item numbers to follow the order in which the assembly appears
in the FeatureManager design tree.

Syntax (OLE Automation)

retval = BomFeature.FollowAssemblyOrder ()

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if the order of the item numbers follows the order in which the assembly appears in the FeatureManager design tree, FALSE if not |

#

Syntax (COM)

status = BomFeature->FollowAssemblyOrder ( &retval)

|  |  |  |
| --- | --- | --- |
| Output: | (VARIANT\_BOOL) retval | TRUE if the order of the item numbers follows the order in which the assembly appears in the FeatureManager design tree, FALSE if not |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks