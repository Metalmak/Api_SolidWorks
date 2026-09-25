<!-- source: swconst/ViewUserInterface.htm -->

# SOLIDWORKS API Help

# View > User Interface

![](ViewUserInterface.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Dynamic Reference Visualization (Parent) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDynamicReferenceVisualization\_Parent)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDynamicReferenceVisualization\_Parent, <OnFlag>) | Boolean value | Specifies whether to display parent relationships |
| Dynamic Reference Visualization (Child) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDynamicReferenceVisualization\_Child)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDynamicReferenceVisualization\_Child, <OnFlag>) | Boolean value | Specifies whether to display child relationships |