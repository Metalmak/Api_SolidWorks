<!-- source: swconst/SO_Drawings-Performance.htm -->

# SOLIDWORKS API Help

# System Options > Drawings > Performance

![](SO_Drawings-Performance.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Show contents while dragging drawing view | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDrawingViewShowContentsWhileDragging)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDrawingViewShowContentsWhileDragging, <OnFlag>) | Boolean value | Specifies whether model or view boundary is displayed when view is dragged |
| Allow auto-update when opening drawings | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutomaticDrawingViewUpdateDefault  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutomaticDrawingViewUpdateDefault, <OnFlag>) | Boolean value | Specifies whether drawing views are updated when a drawing is opened |
| Save tessellated data for drawings with shaded and draft quality views | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDrawingSaveShadedData)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDrawingSaveShadedData, <OnFlag>) | Boolean value | Specifies whether to save tessellated data in drawing documents with shaded and draft quality views |
| Turn Off Automatic Solve Mode and Undo and turn on No Solve Mode when drawing view contains more than... | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDrawingTurnOffAutomaticSolveModeAndUndo)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDrawingTurnOffAutomaticSolveModeAndUndo, <OnFlag>) | Boolean value | True to turn off Automatic Solve Mode and Undo and turn on No Solve Mode when drawing view contains more than the specified number of sketch entities False to turn on Automatic Solve Mode and Undo and turn off No Solve Mode when drawing view contains more than the specified number of sketch entities |
| this number of sketch entities | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDrawing\_Auto\_Solve\_Threshold) ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swDrawing\_Auto\_Solve\_Threshold, <*Value*>) | Integer value | The specified number of sketch entities mentioned in the previous comment |