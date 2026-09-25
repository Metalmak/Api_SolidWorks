<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~SetMultipleFilenamesPrompt.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetMultipleFilenamesPrompt Method (ISldWorks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html) : SetMultipleFilenamesPrompt Method (ISldWorks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Array of filenames

Sets the new filenames to open in response to the ISldWorks [PromptForMultipleFileNamesNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DSldWorksEvents_PromptForMultipleFileNamesNotifyEventHandler.html) event.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetMultipleFilenamesPrompt( _    ByVal FileName As System.Object _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ISldWorks Dim FileName As System.Object   instance.SetMultipleFilenamesPrompt(FileName) ``` | |

| C# |  |
| --- | --- |
| ``` void SetMultipleFilenamesPrompt(     System.object FileName ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetMultipleFilenamesPrompt(  &   System.Object^ FileName ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*FileName*
:   Array of filenames

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See SldWorks::SetMultipleFilenamesPrompt.

# ![](dotnetimages/collapse.gif)Remarks

The filenames specified are only used if the SOLIDWORKS [PromptForMultipleFileNamesNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DSldWorksEvents_PromptForMultipleFileNamesNotifyEventHandler.html) event returns S\_FALSE. This implies that you cannot specify initial filenames for SOLIDWORKS to use in the standard dialog. Instead, you must provide your own file dialog and return the filenames after the user selects them.

Guidelines for using this method when the cause argument of the SOLIDWORKS PromptForMultipleFileNamesNotify event is set to swSaveVirtualComponentExternally:

* Length of the Filename argument array must be equal to the length of the suggestedFileNames argument array passed into ISldWorks::SetMultipleFilenamesPrompt. If there is a mismatch, all virtual components will be saved internal to the assembly with the suggested file name passed by the SOLIDWORKS PromptForMultipleFileNamesNotify event .* Supplying a full path and file name will save a virtual component external to the assembly using that path and file name.* Supplying only a file name (i.e., no path) will save the virtual component internal to the assembly with the suggested file name passed by the SOLIDWORKS PromptForMultipleFileNamesNotify event .* This method cannot be used to change the name of an internally saved virtual component.* Supplying an empty string will save the virtual component external to the assembly and in the same folder as the assembly with the suggested file name passed by the SOLIDWORKS PromptForMultipleFileNamesNotify event.* Supplying an invalid path and file name or insufficient access rights will save the virtual component internal to the assembly with the suggested file name passed by the SOLIDWORKS PromptForMultipleFileNamesNotify event.* Insufficient access rights to the path and file name will save the virtual component internal to the assembly with the suggested file name passed by the SOLIDWORKS PromptForMultipleFileNamesNotify event.

# ![](dotnetimages/collapse.gif)See Also

####

[ISldWorks Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks.html)

[ISldWorks Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks_members.html)

[ISldWorks::SetNewFilename Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~SetNewFilename.html)

[ISldWorks::SetPromptFilename Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ISldWorks~SetPromptFilename.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 SP1, Revision Number 16.0