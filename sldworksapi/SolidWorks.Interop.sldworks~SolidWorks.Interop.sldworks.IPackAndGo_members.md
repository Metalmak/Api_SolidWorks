<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo_members.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IPackAndGo Interface Members | |
| [See Also](#seealsobookmark)  [Properties](#PropertiesBookmark)  [Methods](#MethodsBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : IPackAndGo Interface |

The following tables list the members exposed by [IPackAndGo](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo.html).

# ![](dotnetimages/collapse.gif)Public Properties

|  | Name | Description |
| --- | --- | --- |
| ![ Property](dotnetimages/Property.gif) | [AddPrefix](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~AddPrefix.html) | Gets or sets a prefix for all filenames for Pack and Go. |
| ![ Property](dotnetimages/Property.gif) | [AddSuffix](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~AddSuffix.html) | Gets or sets a suffix for all filenames for Pack and Go. |
| ![ Property](dotnetimages/Property.gif) | [FlattenToSingleFolder](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~FlattenToSingleFolder.html) | Gets or sets whether to save all files to the root directory of the Pack and Go destination folder. |
| ![ Property](dotnetimages/Property.gif) | [IncludeDrawings](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~IncludeDrawings.html) | Gets or sets whether to add the model's drawing documents to Pack and Go. |
| ![ Property](dotnetimages/Property.gif) | [IncludeSimulationResults](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~IncludeSimulationResults.html) | Gets or sets whether to add the model's SOLIDWORKS Simulation results to Pack and Go. |
| ![ Property](dotnetimages/Property.gif) | [IncludeSuppressed](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~IncludeSuppressed.html) | Gets or sets whether to included suppressed components in Pack and Go. |
| ![ Property](dotnetimages/Property.gif) | [IncludeToolboxComponents](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~IncludeToolboxComponents.html) | Gets or sets whether to include SOLIDWORKS Toolbox components in Pack and Go. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)Public Methods

|  | Name | Description |
| --- | --- | --- |
| ![ Method](dotnetimages/Method.gif) | [AddExternalDocuments](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~AddExternalDocuments.html) | Adds non-SOLIDWORKS files to Pack and Go. |
| ![ Method](dotnetimages/Method.gif) | [GetDocumentNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~GetDocumentNames.html) | Gets the original paths and filenames of all of the model's documents for Pack and Go. |
| ![ Method](dotnetimages/Method.gif) | [GetDocumentNamesCount](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~GetDocumentNamesCount.html) | Gets the number of documents comprising the model for Pack and Go. |
| ![ Method](dotnetimages/Method.gif) | [GetDocumentSaveToNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~GetDocumentSaveToNames.html) | Gets the paths and filenames to which to save the model's documents for Pack and Go set by [IPackAndGo::SetDocumentSaveToNames](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPackAndGo~SetDocumentSaveToNames.html). |
| ![ Method](dotnetimages/Method.gif) | [GetExternalDocuments](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~GetExternalDocuments.html) | Gets the paths and filenames of the non-SOLIDWORKS files added to Pack And Go. |
| ![ Method](dotnetimages/Method.gif) | [GetSaveToName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~GetSaveToName.html) | Gets the path or the path and filename of the Zip file for Pack and Go set by [IPackAndGo::SetSaveToName](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPackAndGo~SetSaveToName.html). |
| ![ Method](dotnetimages/Method.gif) | [IGetDocumentNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~IGetDocumentNames.html) | Gets the original paths and filenames of all of the model's documents for Pack and Go. |
| ![ Method](dotnetimages/Method.gif) | [IGetDocumentSaveToNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~IGetDocumentSaveToNames.html) | Gets the paths and filenames to which to save the model's documents for Pack and Go set by [IPackAndGo::ISetDocumentSaveToNames](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPackAndGo~ISetDocumentSaveToNames.html). |
| ![ Method](dotnetimages/Method.gif) | [ISetDocumentSaveToNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~ISetDocumentSaveToNames.html) | Sets the paths and filenames of the documents to save in Pack and Go. |
| ![ Method](dotnetimages/Method.gif) | [RemoveExternalDocuments](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~RemoveExternalDocuments.html) | Removes the specified non-SOLIDWORKS files from Pack and Go. |
| ![ Method](dotnetimages/Method.gif) | [SetDocumentSaveToNames](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~SetDocumentSaveToNames.html) | Sets the paths and filenames of the documents for Pack and Go. |
| ![ Method](dotnetimages/Method.gif) | [SetSaveToName](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~SetSaveToName.html) | Overrides the paths and filenames of the documents set by [IPackAndGo::SetDocumentSaveToNames](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPackAndGo~SetDocumentSaveToNames.html) or [IPackAndGo::ISetDocumentSaveToNames](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IPackAndGo~ISetDocumentSaveToNames.html) with the specified path or the path and name of the Zip file. |

[Top](#topBookmark)

# ![](dotnetimages/collapse.gif)See Also

####

[IPackAndGo Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo.html)

[SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html)