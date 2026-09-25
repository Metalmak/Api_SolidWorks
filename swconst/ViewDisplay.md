<!-- source: swconst/ViewDisplay.htm -->

# SOLIDWORKS API Help

# View > Display

![](ViewDisplay.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Ambient Occlusion | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayAmbientOcclusionShadows)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swDisplayAmbientOcclusionShadows, <OnFlag>) | Boolean value | Specifies whether to use global lighting that adds realism to models by controlling the attenuation of ambient light due to occluded areas; available in all scenes when you use RealView graphics |