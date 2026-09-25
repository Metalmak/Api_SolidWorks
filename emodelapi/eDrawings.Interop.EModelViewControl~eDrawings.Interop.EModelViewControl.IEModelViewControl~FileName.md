<!-- source: emodelapi/eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl~FileName.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| eDrawings API Help | Send comments on this topic. |
| FileName Property (IEModelViewControl) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [eDrawings.Interop.EModelViewControl Namespace](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl_namespace.html) > [IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html) : FileName Property (IEModelViewControl) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets the path and name of the file to open or the file name of the currently displayed file.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property FileName As System.String ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IEModelViewControl Dim value As System.String   instance.FileName = value   value = instance.FileName ``` | |

| C# |  |
| --- | --- |
| ``` System.string FileName {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.String^ FileName {    System.String^ get();    void set ( &   System.String^ value); } ``` | |

#### Property Value

Fully qualified path and file name (see Remarks)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EModelViewControl::FileName.

# ![](dotnetimages/collapse.gif)Remarks

Syntax for specifying the file name:

|  |  |
| --- | --- |
| Access | Example |
| Windows local file | C:\temp\myAssembly.easm |
| Windows network path | //myServer//mySharedFolder//myDrawing.edrw   (Assume that the folder is shared and note the use of the forward slashes) |
| URL | Supported: http://myHost/MyFolder/MyPart.eprt  Not supported: file:///C:/temp\myDwg.dwg |

# ![](dotnetimages/collapse.gif)See Also

####

[IEModelViewControl Interface](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl.html)

[IEModelViewControl Members](eDrawings.Interop.EModelViewControl~eDrawings.Interop.EModelViewControl.IEModelViewControl_members.html)

# ![](dotnetimages/collapse.gif)Availability

eDrawings API 2005 SP0