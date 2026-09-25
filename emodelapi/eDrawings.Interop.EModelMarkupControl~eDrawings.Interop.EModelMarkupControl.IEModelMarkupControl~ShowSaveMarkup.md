<!-- source: emodelapi/eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl~ShowSaveMarkup.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| ShowSaveMarkup Method (IEModelMarkupControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelMarkupControl Namespace](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl_namespace.html) > [IEModelMarkupControl Interface](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl.html) : ShowSaveMarkup Method (IEModelMarkupControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*SaveName*
:   Name of  the file where to save the markup comments

*SaveAs*
:   |  |  |
    | --- | --- |
    | If... | Then.. |
    | TRUE | A dialog is displayed prompting the user to select the markup to save and the file name to which to save the markup. SaveName is ignored. |
    | FALSE | |  |  | | --- | --- | | **If...** | **Then markups from all reviewers are saved to...** | | SaveName is empty | The default file name in the current directory | | SaveName is specified | The file specified in SaveName | |

Saves the markup comments to either the specified file or to the default markup file.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub ShowSaveMarkup( _    ByVal SaveName As System.String, _    ByVal SaveAs As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEModelMarkupControl Dim SaveName As System.String Dim SaveAs As System.Boolean   instance.ShowSaveMarkup(SaveName, SaveAs) ``` | |

| C# |  |
| --- | --- |
| ``` void ShowSaveMarkup(     System.string SaveName,    System.bool SaveAs ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void ShowSaveMarkup(  &   System.String^ SaveName, &   System.bool SaveAs ) ``` | |

#### Parameters

*SaveName*
:   Name of  the file where to save the markup comments

*SaveAs*
:   |  |  |
    | --- | --- |
    | If... | Then.. |
    | TRUE | A dialog is displayed prompting the user to select the markup to save and the file name to which to save the markup. SaveName is ignored. |
    | FALSE | |  |  | | --- | --- | | **If...** | **Then markups from all reviewers are saved to...** | | SaveName is empty | The default file name in the current directory | | SaveName is specified | The file specified in SaveName | |

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EModelMarkupControl::ShowSaveMarkup.

# ![](dotnetimages/collapse.gif)Example

See the [IEModelMarkupControl](eDrawings.Interop.EModelMarkupControl.html) examples.

# ![](dotnetimages/collapse.gif)See Also

####

[IEModelMarkupControl Interface](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl.html)

[IEModelMarkupControl Members](eDrawings.Interop.EModelMarkupControl~eDrawings.Interop.EModelMarkupControl.IEModelMarkupControl_members.html)

[IEModelViewControl::IsMarkupModified](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~IsMarkupModified.html)

[IEModelViewControl::OpenMarkupFile](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~OpenMarkupFile.html)

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2005 SP0