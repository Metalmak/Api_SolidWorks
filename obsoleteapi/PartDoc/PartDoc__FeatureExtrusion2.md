<!-- source: obsoleteapi/PartDoc/PartDoc__FeatureExtrusion2.htm -->

# PartDoc::FeatureExtrusion2

This method is obsolete and has been superseded
by [PartDoc::FeatureExtrusion3](PartDoc__FeatureExtrusion3.htm).

Description

This method creates an extrusion to use as a base feature.

Syntax (OLE Automation)

void PartDoc.FeatureExtrusion2 ( sd, flip, dir, t1,
t2, d1, d2, dchk1, dchk2, ddir1, ddir2, dang1, dang2, offsetReverse1,
offsetReverse2, merge)

| Input: | (BOOL) sd | TRUE for single-ended, FALSE for double-ended |
| Input: | (BOOL) flip | TRUE to flip the direction to cut |
| Input: | (BOOL) dir | TRUE to flip direction to extrude |
| Input: | (long) t1 | Termination type for first end as defined in swEndConditions\_e |
| Input: | (long) t2 | Termination type for second end as defined in swEndConditions\_e |
| Input: | (double) d1 | Depth of extrusion for first end in meters |
| Input: | (double) d2 | Depth of extrusion for second end in meters |
| Input: | (BOOL) dchk1 | TRUE allows draft angle in first direction, FALSE does not allow drafting |
| Input: | (BOOL) dchk2 | TRUE allows draft angle in second direction, FALSE does not allow drafting |
| Input: | (BOOL) ddir1 | For first draft angle to be inward use TRUE, for draft angle outward use FALSE |
| Input: | (BOOL) ddir2 | For second draft angle to be inward use TRUE, for draft angle outward use FALSE |
| Input: | (double) dang1 | Draft angle for first end |
| Input: | (double) dang2 | Draft angle for second end |
| Input: | (BOOL) offsetReverse1 | If you chose to offset the first end condition from another face or plane, then TRUE specifies offset in direction away from the sketch, FALSE specifies offset from the face or plane in a direction toward the sketch |
| Input: | (BOOL) offsetReverse2 | If you chose to offset the second end condition from another face or plane, th3n TRUE specifies offset in direction away from the sketch, FALSE specifies offset from the face or plane in a direction toward the sketch |
| Input: | (BOOL) merge | TRUE to merge the feature, FALSE otherwise |

Syntax (COM)

status = PartDoc->FeatureExtrusion2 ( sd, flip,
dir, t1, t2, d1, d2, dchk1, dchk2, ddir1, ddir2, dang1, dang2, offsetReverse1,
offsetReverse2, merge )

| Input: | (VARIANT\_BOOL) sd | TRUE for single-ended, FALSE for double-ended |
| Input: | (VARIANT\_BOOL) flip | TRUE to flip the direction to cut |
| Input: | (VARIANT\_BOOL) dir | TRUE to flip direction to extrude |
| Input: | (long) t1 | Termination type for first end as defined in swEndConditions\_e |
| Input: | (long) t2 | Termination type for second end as defined in swEndConditions\_e |
| Input: | (double) d1 | Depth of extrusion for first end in meters |
| Input: | (double) d2 | Depth of extrusion for second end in meters |
| Input: | (VARIANT\_BOOL) dchk1 | TRUE allows draft angle in first direction, FALSE does not allow drafting |
| Input: | (VARIANT\_BOOL) dchk2 | TRUE allows draft angle in second direction, FALSE does not allow drafting |
| Input: | (VARIANT\_BOOL) ddir1 | For first draft angle to be inward use TRUE, for draft angle outward use FALSE |
| Input: | (VARIANT\_BOOL) ddir2 | For second draft angle to be inward use TRUE, for draft angle outward use FALSE |
| Input: | (double) dang1 | Draft angle for first end |
| Input: | (double) dang2 | Draft angle for second end |
| Input: | (VARIANT\_BOOL) offsetReverse1 | If you chose to offset the first end condition from another face or plane, then TRUE specifies offset in direction away from the sketch, FALSE specifies offset from the face or plane in a direction toward the sketch |
| Input: | (VARIANT\_BOOL) offsetReverse2 | If you chose to offset the second end condition from another face or plane, th3n TRUE specifies offset in direction away from the sketch, FALSE specifies offset from the face or plane in a direction toward the sketch |
| Input: | (VARIANT\_BOOL) merge | TRUE to merge the feature, FALSE otherwise |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks