<!-- source: swconst/FileOpenNonNative.htm -->

# SOLIDWORKS API Help

# File > Open

![](FileOpenNonNative.gif)

| Setting | Get/Set Methods | Return Value  or  <Value>  or  <OnFlag> | Comment |
| Include PMI | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swIncludePMI)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swIncludePMI, <OnFlag>) | Boolean value | Specifies whether to include Product Manufacturing information when opening these non-native file types:  * ACIS * CATIA V5 * ProE/Creo * Unigraphics/NX * Inventor * Solid Edge |