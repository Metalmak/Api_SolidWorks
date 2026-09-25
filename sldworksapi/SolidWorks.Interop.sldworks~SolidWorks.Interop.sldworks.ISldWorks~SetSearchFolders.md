<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~SetSearchFolders.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetSearchFolders Method (ISldWorks) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : SetSearchFolders Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FolderType*
:   The search folder type; the only type currently supported is swDocumentType; for an up-to-date listing, see swSearchFolderTypes\_e

*Folders*
:   String containing all of the search folders; each search folder should be separated by a semicolon

Sets the current folder search path as shown in Tools > Options > System Options > File Locations > Show folders for  > Referenced Documents.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function SetSearchFolders( _    ByVal FolderType As System.Integer, _    ByVal Folders As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim FolderType As System.Integer Dim Folders As System.String Dim value As System.Boolean   value = instance.SetSearchFolders(FolderType, Folders) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool SetSearchFolders(     System.int FolderType,    System.string Folders ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool SetSearchFolders(  &   System.int FolderType, &   System.String^ Folders ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FolderType*
:   The search folder type; the only type currently supported is swDocumentType; for an up-to-date listing, see swSearchFolderTypes\_e

*Folders*
:   String containing all of the search folders; each search folder should be separated by a semicolon

#### Return Value

True if the search folders were set, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::SetSearchFolders.

# ![](dotnetimages/collapse.gif)Example

[Get and Set Search Folders (VBA)](Get_and_Set_Search_Folders_Example_VB.htm)

[Get and Set Search Folders (VB.NET)](Get_and_Set_Search_Folders_Example_VBNET.htm)

[Get and Set Search Folders (C#)](Get_and_Set_Search_Folders_Example_CSharp.htm)

# ![](dotnetimages/collapse.gif)Remarks

The search folders are used by SOLIDWORKS based on their order. Folders at the top of the list get searched first and folders at the bottom of the list get searched last.

This method does not allow you to incrementally add to the search folders list. Calling this method overwrites the existing search folder settings. If you want to add a folder to the existing search folder list, you must get the current search folder list using [ISldWorks::GetSearchFolders](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~GetSearchFolders.html) and then add your folder string at the appropriate location.

Search folder settings are ignored unless **Tools > Options > System Options > External References >** Search file locations for external references is selected. To get and set Search file locations for external references in the SOLIDWORKS API, use swUserPreferenceToggle\_e.swUseFolderSearchRules with [ISldWorks::GetUserPreferenceToggle](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~GetUserPreferenceToggle.html) and [ISldWorks::SetUserPreferenceToggle](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~SetUserPreferenceToggle.html), respectively.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::GetSearchFolders Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetSearchFolders.html)

[ISldWorks::SetMissingReferencePathName Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~SetMissingReferencePathName.html)

[ISldWorks::GetDataFolder Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~GetDataFolder.html)