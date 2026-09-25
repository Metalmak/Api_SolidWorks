<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DSldWorksEvents_PromptForFilenameNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DSldWorksEvents\_PromptForFilenameNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DSldWorksEvents\_PromptForFilenameNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

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

*suggestedFileName*
:   Name of the missing SOLIDWORKS document

*DocType*
:   Type of the missing document as defined in swDocumentTypes\_e

*cause*
:   Cause as defined in swPrompForFilenameCause\_e

Fired when a dependent document is missing from the file being opened.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DSldWorksEvents_PromptForFilenameNotifyEventHandler( _    ByVal openOrSave As System.Integer, _    ByVal suggestedFileName As System.String, _    ByVal DocType As System.Integer, _    ByVal cause As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DSldWorksEvents_PromptForFilenameNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_PromptForFilenameNotifyEventHandler(     System.int openOrSave,    System.string suggestedFileName,    System.int DocType,    System.int cause ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DSldWorksEvents_PromptForFilenameNotifyEventHandler(  &   System.int openOrSave, &   System.String^ suggestedFileName, &   System.int DocType, &   System.int cause ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*openOrSave*
:   * 0 = save* 1 = open

*suggestedFileName*
:   Name of the missing SOLIDWORKS document

*DocType*
:   Type of the missing document as defined in swDocumentTypes\_e

*cause*
:   Cause as defined in swPrompForFilenameCause\_e

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PromptForFilenameNotify Event (SldWorks).

# ![](dotnetimages/collapse.gif)Remarks

Use this event with the [ISldWorks::SetPromptFilename2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~SetPromptFilename2.html) method, not with the [ISldWorks::SetMissingReferencePathName](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ISldWorks~SetMissingReferencePathName.html) method.

An example of a good use for this event is when you are mirroring an assembly. If you want to create new files for the mirrored components, use this notification to specify the new filename. This is useful when you want to choose filenames for the newly created components during the mirroring process.

If developing a C++ application, use swAppPromptForFileNameNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0