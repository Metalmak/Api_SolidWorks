<!-- source: cworksapi/SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Simulation API Help | Send comments on this topic. |
| ICWJoints Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html) : ICWJoints Interface |

The following tables list the members exposed by [ICWJoints](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [IncludeAllSelectedBeam](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints~IncludeAllSelectedBeam.html) | Get or sets whether to include all beams in the joints. |
| ![ Property](dotnetimages/Property.gif) | [IncludeDisplayNeutralAxis](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints~IncludeDisplayNeutralAxis.html) | Gets or sets whether to show or hide a neutral axis for each beam. |
| ![ Property](dotnetimages/Property.gif) | [IncludeKeepModifiedJointOnUpdate](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints~IncludeKeepModifiedJointOnUpdate.html) | Gets or sets whether to save modifications made to the joints. |
| ![ Property](dotnetimages/Property.gif) | [IncludeTreatAsJointForClearanceLessThan](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints~IncludeTreatAsJointForClearanceLessThan.html) | Gets or sets whether to overwrite the optimal tolerance value for non-touching structural members within a certain distance, also called pinballs. |
| ![ Property](dotnetimages/Property.gif) | [IncludeUserSelectedBeam](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints~IncludeUserSelectedBeam.html) | Gets or sets whether to include only the user-selected beams. |
| ![ Property](dotnetimages/Property.gif) | [PinBallRadius](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints~PinBallRadius.html) | Gets or sets the optimal tolerance value for non-touching structural members within a certain distance, which is also referred to as a pinball. |
| ![ Property](dotnetimages/Property.gif) | [PinBallRadiusUnit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints~PinBallRadiusUnit.html) | Gets or sets the unit for the optimal tolerance value for non-touching structural members within a certain distance, which is also referred to as a pinball. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [CalculateJoints](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints~CalculateJoints.html) | Calculates the joints at the free ends of structural members and at the intersection of two or more structural members. |
| ![ Method](dotnetimages/Method.gif) | [DeleteJoint](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints~DeleteJoint.html) | Deletes the specified joint. |
| ![ Method](dotnetimages/Method.gif) | [InsertBeamEntity](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints~InsertBeamEntity.html) | Inserts the specified beam in the joints. |
| ![ Method](dotnetimages/Method.gif) | [JointsBeginEdit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints~JointsBeginEdit.html) | Begins editing of joints. |
| ![ Method](dotnetimages/Method.gif) | [JointsEndEdit](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints~JointsEndEdit.html) | Ends editing of joints. |
| ![ Method](dotnetimages/Method.gif) | [RemoveBeamEntityAt](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints~RemoveBeamEntityAt.html) | Removes the specified beam from the joints. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[ICWJoints Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWJoints.html)

[SolidWorks.Interop.cosworks Namespace](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks_namespace.html)

[ICWBeamBody Interface](SolidWorks.Interop.cosworks~SolidWorks.Interop.cosworks.ICWBeamBody.html)