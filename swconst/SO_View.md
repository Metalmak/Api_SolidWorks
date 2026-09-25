<!-- source: swconst/SO_View.htm -->

# SOLIDWORKS API Help

# System Options > View

![](SO_View.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Reverse mouse wheel zoom direction | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swViewReverseWheelZoomDirection)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swViewReverseWheelZoomDirection, <OnFlag>) | Boolean value | Specifies whether to reverse a mouse's wheel zoom direction |
| Zoom to fit when changing to standard views | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swViewZoomFitAndCenter)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swViewZoomFitAndCenter, <OnFlag>) | Boolean value | Specifies whether to zoom-to-fit view when changing to standard views |
| View rotation - Arrow keys | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swViewRotationArrowKeys)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swViewRotationArrowKeys, <Value>) | Double value in radians | Specifies angle increment for view rotation when arrow keys are used to rotate model |
| View rotation - Mouse speed | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swViewRotationMouseSpeed)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swViewRotationMouseSpeed, <Value>) | Integer value from 1 to 100 | Specifies the speed of rotation when you use the mouse to rotate the model or assembly component |
| Transitions - View transition | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swViewAnimationSpeed)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swViewAnimationSpeed, <Value>) | Double value:   * 0 = off * >0 - 3 seconds | Specifies animation-like speed when changing views |
| Transitions - Hide/show component | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swViewTransitionHideShowComponent)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swViewTransitionHideShowComponent, <Value>) | Double value | Specifies the animation-like speed at which to transition the view when hiding or showing components |
| Transitions - Isolate | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swViewTransitionIsolate)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swViewTransitionIsolate, <Value>) | Double value | Specifies the animation-like speed at which to transition the view when isolating a component in assemblies and multi-body parts |
| Transitions - View selector | ISldWorks::GetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swViewSelectorSpeed)  ISldWorks::SetUserPreferenceDoubleValue(swUserPreferenceDoubleValue\_e.swViewSelectorSpeed, <Value>) | Double value | Specifies the speed of the View selector animation; 0 indicates no animation and the current model is shown in the background; 3.0 is the maximum value |