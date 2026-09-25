<!-- source: obsoleteapi/PartDoc/PartDoc__FeatureExtrusionThin2.htm -->

# PartDoc::FeatureExtrusionThin2

This method is obsolete and has been superseded
by [PartDoc::FeatureExtrusionThin3](PartDoc__FeatureExtrusionThin3.htm).

Description

This method creates an extruded
thin feature by extruding a profile. A constant thickness is given to
profile during extruding.

Syntax (OLE Automation)

void PartDoc.FeatureExtrusionThin2 ( sd, flip, dir,
t1, t2, d1, d2, dchk1, dchk2, ddir1, ddir2, dang1, dang2, offsetReverse1,
offsetReverse2, merge, thk1, thk2, endThk, revThinDir, capEnds, addBends,
bendRad)

|  |  |  |
| --- | --- | --- |
| Input: | (BOOL) sd | TRUE for single-ended, FALSE for double-ended |
| Input: | (BOOL) flip | Not used |
| Input: | (BOOL) dir | reverse direction. TRUE if you want Direction1 to be opposite the default direction |
| Input: | (long) t1 | First end as defined in swEndConditions\_e |
| Input: | (long) t2 | Second end as defined in swEndConditions\_e |
| Input: | (double) d1 | Depth of extrusion for first end in meters |
| Input: | (double) d2 | Depth of extrusion for second end in meters |
| Input: | (BOOL) dchk1 | TRUE allows draft angle in first direction, FALSE does not allow drafting |
| Input: | (BOOL) dchk2 | TRUE allows draft angle in second direction, FALSE doesn't allow drafting |
| Input: | (BOOL) ddir1 | For first draft angle to be inward use TRUE, for draft angle outward use FALSE |
| Input: | (BOOL) ddir2 | For second draft angle to be inward use TRUE, for draft angle outward use FALSE |
| Input: | (double) dang1 | Draft angle for first end |
| Input: | (double) dang2 | Draft angle for second end |
| Input: | (BOOL) offsetReverse1 | If you chose to offset the first end condition from another face or plane, then TRUE specifies offset in direction away from the sketch,  FALSE specifies offset from the face or plane in a direction toward the sketch |
| Input: | (BOOL) offsetReverse2 | If you chose to offset the second end condition from another face or plane, then TRUE specifies offset in direction away from the sketch, FALSE specifies offset from the face or plane in a direction toward the sketch |
| Input: | (BOOL) merge | TRUE merge the feature, FALSE otherwise |
| Input: | (double) thk1 | Wall thickness 1; midplane type uses (thk1)/2 for each direction |
| Input: | (double) thk2 | Wall thickness 2; only used when thinType |
| Input: | (double) endThk | End-cap thickness; only used when capEnds = 1 |
| Input: | (long) revThinDir | Thin feature type:   * 0 = One   direction * 1 = One   direction reverse * 2 = Midplane * 3 = Two   direction |
| Input: | (long) capEnds | Cap the ends:   * 0 = no   cap * 1 = cap   (base features only) |
| Input: | (BOOL) addBends | TRUE to add auto fillets (open profile base features only) |
| Input: | (double) bendRad | Fillet radii if addFillets = TRUE |

Syntax (COM)

status = PartDoc->FeatureExtrusionThin2 ( sd,
flip, dir, t1, t2, d1, d2, dchk1, dchk2, ddir1, ddir2, dang1, dang2, offsetReverse1,
offsetReverse2, merge, thk1, thk2, endThk, revThinDir, capEnds, addBends,
bendRad )

|  |  |  |
| --- | --- | --- |
| Input: | (VARIANT\_BOOL) sd | TRUE for single-ended, FALSE for double-ended |
| Input: | (VARIANT\_BOOL) flip | Not used |
| Input: | (VARIANT\_BOOL) dir | reverse direction. TRUE if you want Direction1  to be opposite the default direction |
| Input: | (long) t1 | First end as defined in swEndConditions\_e |
| Input: | (long) t2 | Second end as defined in swEndConditions\_e |
| Input: | (double) d1 | Depth of extrusion for first end in meters |
| Input: | (double) d2 | Depth of extrusion for second end in meters |
| Input: | (VARIANT\_BOOL) dchk1 | TRUE allows draft angle in first direction, FALSE does not allow drafting |
| Input: | (VARIANT\_BOOL) dchk2 | TRUE allows draft angle in second direction, FALSE doesn't allow drafting |
| Input: | (VARIANT\_BOOL) ddir1 | For first draft angle to be inward use TRUE, for draft angle outward use FALSE |
| Input: | (VARIANT\_BOOL) ddir2 | For second draft angle to be inward use TRUE, for draft angle outward use FALSE |
| Input: | (double) dang1 | Draft angle for first end |
| Input: | (double) dang2 | Draft angle for second end |
| Input: | (VARIANT\_BOOL) offsetReverse1 | If you chose to offset the first end condition from another face or plane, then TRUE specifies offset in direction away from the sketch,  FALSE specifies offset from the face or plane in a direction toward the sketch |
| Input: | (VARIANT\_BOOL) offsetReverse2 | If you chose to offset the second end condition from another face or plane, then TRUE specifies offset in direction away from the sketch, FALSE specifies offset from the face or plane in a direction toward the sketch |
| Input: | (VARIANT\_BOOL) merge | TRUE merge the feature, FALSE otherwise |
| Input: | (double) thk1 | Wall thickness 1; midplane type uses (thk1)/2 for each direction |
| Input: | (double) thk2 | Wall thickness 2; only used when thinType |
| Input: | (double) endThk | End-cap thickness; only used when capEnds = 1 |
| Input: | (long) revThinDir | Thin feature type:   * 0 = One   direction * 1 = One   direction reverse * 2 = Midplane * 3 = Two   direction |
| Input: | (long) capEnds | Cap the ends:   * 0 = no   cap * 1 = cap   (base features only) |
| Input: | (VARIANT\_BOOL) addBends | TRUE to add auto fillets (open profile base features only) |
| Input: | (double) bendRad | Fillet radii if addFillets = TRUE |
| Return: | (HRESULT) status | S\_OK if successful |

Remarks