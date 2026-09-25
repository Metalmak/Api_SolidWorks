<!-- source: swconst/SO_Touch.htm -->

# SOLIDWORKS API Help

# System Options > Touch

![](SO_Touch.gif)

| Setting | Get/Set Methods | Return Value or <*Value*> | Comment |
| Rotate and Pan - Rotate width | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSystemTouchRotateWidth)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSystemTouchRotateWidth, <Value>) | Double value:  * 0 = Interpret the   two-finger gesture as a Pan * >0 = Interpret this maximum initial   two-finger distance as a Rotate |  |
| Rotate and Pan - Rotate versus pan threshold | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSystemTouchRotateVersusPanThreshold)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swSystemTouchRotateVersusPanThreshold, <Value>) | Double value:  * 0 = Interpret any   two-finger distance greater than the **Rotate width** as a Pan * >0 (see **Comment**) | The sum of the non-zero threshold value and the **Rotate width** determines how SOLIDWORKS interprets two-finger gestures:  |  |  | | --- | --- | | When the two-finger distance is... | SOLIDWORKS... | | Less than the sum and greater than the **Rotate width** | Does not interpret the gesture | | Greater than the sum | Interprets the gesture as a Pan | | Less than the **Rotate width** | Interprets the gesture as a Rotate | |
| Automatically pop up Selection tool while hunting for precise location | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutomaticallyPopupSelectionToolForPreciseLocation)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swAutomaticallyPopupSelectionToolForPreciseLocation, <OnFlag>) | Boolean value |  |