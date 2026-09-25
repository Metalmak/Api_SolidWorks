<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DSldWorksEvents_PromptForMultipleFileNamesNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DSldWorksEvents\_PromptForMultipleFileNamesNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DSldWorksEvents\_PromptForMultipleFileNamesNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*openOrSave*
:   * 0 = save* 1 = open

*suggestedFileNames*
:   Array of names of the missing SOLIDWORKS documents

*DocTypes*
:   Types of the missing documents as defined in swDocumentTypes\_e

*cause*
:   Cause as defined in swPrompForFilenameCause\_e

Fired when any dependent documents are missing from the file being opened.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DSldWorksEvents_PromptForMultipleFileNamesNotifyEventHandler( _    ByVal openOrSave As System.Integer, _    ByRef suggestedFileNames As System.Object, _    ByRef DocTypes As System.Object, _    ByVal cause As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DSldWorksEvents_PromptForMultipleFileNamesNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_PromptForMultipleFileNamesNotifyEventHandler(     System.int openOrSave,    ref System.object suggestedFileNames,    ref System.object DocTypes,    System.int cause ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_PromptForMultipleFileNamesNotifyEventHandler(  &   System.int openOrSave, &   System.Object^% suggestedFileNames, &   System.Object^% DocTypes, &   System.int cause ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*openOrSave*
:   * 0 = save* 1 = open

*suggestedFileNames*
:   Array of names of the missing SOLIDWORKS documents

*DocTypes*
:   Types of the missing documents as defined in swDocumentTypes\_e

*cause*
:   Cause as defined in swPrompForFilenameCause\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PromptForMultipleFileNamesNotify Event (SldWorks).

# ![](dotnetimages/collapse.gif)Remarks

Use this event with the [ISldWorks::SetMultipleFilenamesPrompt](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~SetMultipleFilenamesPrompt.html) method.

If developing a C++ application, use swAppPromptForMultipleFileNameNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 SP1, Revision Number 16.1