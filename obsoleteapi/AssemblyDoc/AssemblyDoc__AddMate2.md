<!-- source: obsoleteapi/AssemblyDoc/AssemblyDoc__AddMate2.htm -->

# AssemblyDoc::AddMate2

This method is obsolete and has been superseded
by AssemblyDoc::AddMate3.

Description

This method adds a mate relationship
to the selected entities.

Syntax (OLE Automation)

pMateObjOut = AssemblyDoc.AddMate2 ( mateTypeFromEnum,
alignFromEnum, flip, distance, distAbsUpperLimit, distAbsLowerLimit, gearRatioNumerator,
gearRatioDenominator, angle, angleAbsUpperLimit, angleAbsLowerLimit, errorStatus
)

#

|  |  |  |
| --- | --- | --- |
| Input: | (long) mateTypeFromEnum | Type of mate as defined in swMateType\_e |
| Input: | (long) alignFromEnum | Type of alignment as defined in swMateAlign\_e |
| Input: | (VARIANT\_BOOL) flip | TRUE to flip the component, FALSE otherwise |
| Input: | (double) distance | Distance value to use with distance or limit mates |
| Input: | (double) distAbsUpperLimit | Absolute maximum distance value (see Remarks) |
| Input: | (double) distAbsLowerLimit | Absolute minimum distance value  (see Remarks) |
| Input: | (double) gearRatioNumerator | Gear ratio numerator value for gear mates |
| Input: | (double) gearRatioDenominator | Gear ratio denominator value for gear mates |
| Input: | (double) angle | Angle value to use with angle mates |
| Input: | (double) angleAbsUpperLimit | Absolute maximum angle value |
| Input: | (double) angleAbsLowerLimit | Absolute minimum angle value |
| Output: | (long) errorStatus | Success or error as defined by swAddMateError\_e |
| Output: | (LPMATE2) pMateObjOut | Pointer to the Mate2 object |

#

Syntax (COM)

status = AssemblyDoc->AddMate2 ( mateTypeFromEnum,
alignFromEnum, flip, distance, distAbsUpperLimit, distAbsLowerLimit, gearRatioNumerator,
gearRatioDenominator, angle, angleAbsUpperLimit, angleAbsLowerLimit, errorStatus,
&pMateObjOut )

|  |  |  |
| --- | --- | --- |
| Input: | (long) mateTypeFromEnum | Type of mate as defined in swMateType\_e |
| Input: | (long) alignFromEnum | Type of alignment as defined in swMateAlign\_e |
| Input: | (VARIANT\_BOOL) flip | TRUE to flip the component, FALSE otherwise |
| Input: | (double) distance | Distance value to use with distance or limit mates |
| Input: | (double) distAbsUpperLimit | Absolute maximum distance value (see Remarks) |
| Input: | (double) distAbsLowerLimit | Absolute minimum distance value (see Remarks) |
| Input: | (double) gearRatioNumerator | Gear ratio numerator value for gear mates |
| Input: | (double) gearRatioDenominator | Gear ratio denominator value for gear mates |
| Input: | (double) angle | Angle value to use with angle mates |
| Input: | (double) angleAbsUpperLimit | Absolute maximum angle value |
| Input: | (double) angleAbsLowerLimit | Absolute minimum angle value |
| Output: | (long) errorStatus | Success or error as defined by swAddMateError\_e |
| Output: | (LPMATE2) pMateObjOut | Pointer to the Mate2 object |
| Return: | (HRESULT) status | S\_OK if successful |

#

Remarks

To specify a distance mate
without limits, set the distAbsUpperLimit and distAbsLowerLimit arguments
equal to the distance argument's value.

If mateTypeFromEnum is swMateDISTANCE
or swMateANGLE when the mate is applied to the closest position that meets
the mate condition specified by distance or angle, then setting flip to
TRUE moves the assembly to the other possible mate position.

Use:

* ModelDoc2::ClearSelection2(VARIANT\_TRUE)
  before selecting entities to mate.
* ModelDocExtension::SelectByID2
  with Mark = 1 to select entities to mate.
* ModelDoc2::ClearSelection2(VARIANT\_TRUE)
  after the mate is created.

If mateTypeFromEnum is swMateCAMFOLLOWER,
then use a selection mark of 8 for the cam-follower face.

If nothing is preselected, then errorStatus
is swAddMateError\_IncorrectSeletions and pMateObjOut is NULL/Nothing.