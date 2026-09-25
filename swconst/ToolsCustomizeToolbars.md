<!-- source: swconst/ToolsCustomizeToolbars.htm -->

# SOLIDWORKS API Help

# Tools > Customize > Toolbars

This topic contains two tables. The information in the table:

* appearing immediately after the screen capture
  of the dialog corresponds to the settings on
  that dialog.
titled [Obsolete
Enumerators](#Obsolete) contains enumerators that previously appeared on
the dialog but are now obsolete.

![](ToolsCustomizeToolbars.gif)

| Setting | Get/Set Methods | Return Value or <Value> or <OnFlag> | **Comments** |
| Options - Icon size | ISldWorks::GetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swButtonSize)  ISldWorks::SetUserPreferenceIntegerValue(swUserPreferenceIntegerValue\_e.swButtonSize, swButtonSize\_e.<Value>) | See swButtonSize\_e for valid options |  |

Obsolete Enumerators

| Enumerator | Comment |
| swTextSizeUseOperatingSystemScale | Obsolete; specified whether to use operating system scale |
| swTextSize | Obsolete; specified the text size |