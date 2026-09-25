<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetSearchFolders.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetSearchFolders Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : GetSearchFolders Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FolderType*
:   Search folder type; the only type supported is swDocumentType; for an up-to-date listing, see swSearchFolderTypes\_e

Gets the current folder search path as shown in Tools > Options > System Options > File Locations > Show folders for > Referenced Documents.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetSearchFolders( _    ByVal FolderType As System.Integer _ ) As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim FolderType As System.Integer Dim value As System.String   value = instance.GetSearchFolders(FolderType) ``` | |

| C# |  |
| --- | --- |
| ``` System.string GetSearchFolders(     System.int FolderType ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.String^ GetSearchFolders(  &   System.int FolderType ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FolderType*
:   Search folder type; the only type supported is swDocumentType; for an up-to-date listing, see swSearchFolderTypes\_e

#### Return Value

String containing all of the search folders; each search folder is separated by a semicolon

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::GetSearchFolders.

# ![](dotnetimages/collapse.gif)Example

[Get and Set Search Folders (VBA)](Get_and_Set_Search_Folders_Example_VB.htm)

[Get and Set Search Folders (VB.NET)](Get_and_Set_Search_Folders_Example_VBNET.htm)

[Get and Set Search Folders (C#)](Get_and_Set_Search_Folders_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

Search folder settings are ignored unless **Tools > Options > System Options > External References >** Search file locations for external references is selected. To get and set Search file locations for external references in the SOLIDWORKS API, use swUserPreferenceToggle\_e.swUseFolderSearchRules with [ISldWorks::GetUserPreferenceToggle](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~GetUserPreferenceToggle.html) and [ISldWorks::SetUserPreferenceToggle](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~SetUserPreferenceToggle.html), respectively.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::SetSearchFolders Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~SetSearchFolders.html)

[ISldWorks::GetDataFolder Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetDataFolder.html)

[ISldWorks::SetMissingReferencePathName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~SetMissingReferencePathName.html)