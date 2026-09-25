<!-- source: swconst/SO_FileExplorer.htm -->

# SOLIDWORKS API Help

# System Options > File Explorer

The File Explorer settings are not supported in SOLIDWORKS Connected.

![](SO_FileExplorer.gif)

| Setting | Get/Set Methods | Return Value  or  <OnFlag> | Comment |
| Show in File Explorer view - My Documents (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swFileExplorerShowMyDocuments) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swFileExplorerShowMyDocuments, <OnFlag>) | Boolean value | Specifies whether to show My Documents folder in SOLIDWORKS File Explorer |
| Show in File Explorer view - My Computer (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swFileExplorerShowMyComputer) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swFileExplorerShowMyComputer, <OnFlag>) | Boolean value | Specifies whether to show My Computer folder in SOLIDWORKS File Explorer |
| Show in File Explorer view - My Network Places (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swFileExplorerShowMyNetworkPlaces) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swFileExplorerShowMyNetworkPlaces, <OnFlag>) | Boolean value | Specifies whether to show My Documents folder in SOLIDWORKS File Explorer |
| Show in File Explorer view - Recent Documents (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swFileExplorerShowRecentDocuments) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swFileExplorerShowRecentDocuments, <OnFlag>) | Boolean value | Specifies whether to show My Documents folder in SOLIDWORKS File Explorer |
| Show in File Explorer view - Hidden referenced documents (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swFileExplorerShowHiddenReferencedDocuments) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swFileExplorerShowHiddenReferencedDocuments, <OnFlag>) | Boolean value | Specifies whether to show assembly components that are in memory, but are not open, in the Open in SOLIDWORKS folder in SOLIDWORKS File Explorer |
| Show in File Explorer view - Samples (Not supported in SOLIDWORKS Connected) | ISldWorks::GetUserPreferenceToggle(swUserPreferenceToggle\_e.swFileExplorerShowSamples) ISldWorks::SetUserPreferenceToggle(swUserPreferenceToggle\_e.swFileExplorerShowSamples, <OnFlag>) | Boolean value | Specifies whether to show the Sample folders, which contains online tutorial and What's New sample files, in SOLIDWORKS File Explorer |