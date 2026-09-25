<!-- source: swconst/FileOpenOptionsIDF.htm -->

# SOLIDWORKS API Help

# System Options > Import > IDF

To display the dialog:

Click **Tools > Options > System Options > Import > IDF** in **File
Format**.

- or -

1. Click **File > Open**.
2. In **Files of type**, select **IDF**.
3. Click **Options**.

![](FileOpenOptionsIDF.gif)

| Setting | Get/Set Methods | Return Value  or  <OnFlag> | Comment |
| Add board drilled holes | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportIDFAddDrilledHoles)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportIDFAddDrilledHoles. <OnFlag>) | Boolean value | Specifies whether to add drilled holes from the circuit board; for Intermediate Data Format (IDF) circuit boards files only |
| Reverse underside components | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportIDFReverseUndersideComponents)  ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swImportIDFReverseUndersideComponents. <OnFlag>) | Boolean value | Specifies whether to compensate for incorrectly rotated components by allowing proper location of the component features; for Intermediate Data Format (IDF) circuit board files only |