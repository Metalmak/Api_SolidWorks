<!-- source: swconst/SO_SpinBoxIncrements.htm -->

# SOLIDWORKS API Help

# System Options > Spin Box Increments

![](SO_SpinBoxIncrements.gif)

| Setting | Get/Set Methods | Return Value  or  <Value> | Comment |
| Length increments - English units | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSpinBoxEnglishLengthIncrement)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSpinBoxEnglishLengthIncrement, <Value>) | Double value in inches | Specifies number of inches added or subtracted when spin box arrow is clicked to change a linear dimension value; see [Units](DP_Units.htm) to learn how to set length units using the SOLIDWORKS API |
| Length increments - Metric units | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSpinBoxMetricLengthIncrement)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSpinBoxMetricLengthIncrement, <Value>) | Double value in metric units | Specifies number of units added or subtracted when a spin box arrow is clicked to change a linear dimension value; see [Units](DP_Units.htm) to learn how to set length units using the SOLIDWORKS API |
| Angle increments | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSpinBoxAngleIncrement)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSpinBoxAngleIncrement, <Value>) | Double value in angular units | Specifies number of angular units added or subtracted when a spin box arrow is clicked to change an angular dimension value; see [Units](DP_Units.htm) to learn how to set angular units using the SOLIDWORKS API |
| Time increments | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSpinBoxTimeIncrement)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSpinBoxTimeIncrement, <Value>) | Double value in time units | Specifies number of units added or subtracted when a spin box arrow is clicked to change a time value; see [Units](DP_Units.htm) to learn how to set time units using the SOLIDWORKS API |