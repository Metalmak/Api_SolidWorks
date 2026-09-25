<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~OpenDoc.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| OpenDoc Method (IEModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) > [IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html) : OpenDoc Method (IEModelViewControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*FileName*
:   Fully qualified path and file name (see Remarks)

*IsTemp*
:   True to delete the local copy of a remote non-eDrawings file when that file is closed, false to keep the local copy

*PromptToSave*
:   True to show a dialog if the user exits without saving the file, false to not show a dialog

*ReadOnly*
:   True if the file is read-only, false if not

*CommandString*
:   Specify an empty string (""); do not specify Nothing, Empty, or vbNullString

Opens the specified eDrawings file.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub OpenDoc( _    ByVal FileName As System.String, _    ByVal IsTemp As System.Boolean, _    ByVal PromptToSave As System.Boolean, _    ByVal ReadOnly As System.Boolean, _    ByVal CommandString As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEModelViewControl Dim FileName As System.String Dim IsTemp As System.Boolean Dim PromptToSave As System.Boolean Dim ReadOnly As System.Boolean Dim CommandString As System.String   instance.OpenDoc(FileName, IsTemp, PromptToSave, ReadOnly, CommandString) ``` | |

| C# |  |
| --- | --- |
| ``` void OpenDoc(     System.string FileName,    System.bool IsTemp,    System.bool PromptToSave,    System.bool ReadOnly,    System.string CommandString ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void OpenDoc(  &   System.String^ FileName, &   System.bool IsTemp, &   System.bool PromptToSave, &   System.bool ReadOnly, &   System.String^ CommandString ) ``` | |

#### Parameters

*FileName*
:   Fully qualified path and file name (see Remarks)

*IsTemp*
:   True to delete the local copy of a remote non-eDrawings file when that file is closed, false to keep the local copy

*PromptToSave*
:   True to show a dialog if the user exits without saving the file, false to not show a dialog

*ReadOnly*
:   True if the file is read-only, false if not

*CommandString*
:   Specify an empty string (""); do not specify Nothing, Empty, or vbNullString

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EModelViewControl::OpenDoc.

# ![](dotnetimages/collapse.gif)Example

See [IEModelViewControl](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html) examples.

# ![](dotnetimages/collapse.gif)Remarks

Syntax for specifying the file name:

|  |  |
| --- | --- |
| Access | Example |
| Windows local file | C:\temp\myAssembly.easm |
| Windows network path | //myServer//mySharedFolder//myDrawing.edrw   (Assume that the folder is shared and note the use of the forward slashes) |
| URL | Supported: http://myHost/MyFolder/MyPart.eprt  Not supported: file:///C:/temp\myDwg.dwg |

Because IEModelViewControl::OpenDoc starts a new thread of execution and because eDrawings files are often loaded across the Internet or other potentially slow and unreliable networks, this API call can return before the document is finished loading.

Referencing a model that has not finished loading (for example, calling [IEModelViewControl::Animate](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~Animate.html)) can cause your application to hang, crash, or behave unpredictably. Therefore, listen for the [OnFinishedLoadingDocument](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnFinishedLoadingDocumentEventHandler.html) event after calling IEModelViewControl::OpenDoc so that your application knows when the eDrawings file is finished loading. Once your application receives notification that the eDrawings file has been loaded, it is safe to access the model.

# ![](dotnetimages/collapse.gif)See Also

####

[IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html)

[IEModelViewControl Members](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl_members.html)

[IEModelViewControl::CloseActiveDoc Method](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~CloseActiveDoc.html)

[IEModelViewControl::Save Method](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~Save.html)

[\_IEModelViewControlEvents\_OnFailedLoadingDocumentEventHandler Delegate](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnFailedLoadingDocumentEventHandler.html)

[\_IEModelViewControlEvents\_OnFailedSavingDocumentEventHandler Delegate](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnFailedSavingDocumentEventHandler.html)

[\_IEModelViewControlEvents\_OnFinishedSavingDocumentEventHandler Delegate](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl._IEModelViewControlEvents_OnFinishedSavingDocumentEventHandler.html)

[IEModelViewControl::UserName Property](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~UserName.html)

[IEModelViewControl::Password Property](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~Password.html)

[IEmodelViewControl::AlwaysShowWarningWatermark Property](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~AlwaysShowWarningWatermark.html)

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2005 SP0