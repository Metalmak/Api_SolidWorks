<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.DDrawingDocEvents_EquationEditorPostNotifyEventHandler.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DDrawingDocEvents\_EquationEditorPostNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) : DDrawingDocEvents\_EquationEditorPostNotifyEventHandler Delegate (SolidWorks.Interop.sldworks) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Changed*
:   True if equations have changed, false if not

Notifies your application that the equation editor is being destroyed.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Public Delegate Function DDrawingDocEvents_EquationEditorPostNotifyEventHandler( _    ByVal Changed As System.Boolean _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As New DDrawingDocEvents_EquationEditorPostNotifyEventHandler(AddressOf HandlerMethod) ``` | |

| C# |  |
| --- | --- |
| ``` public delegate System.int DDrawingDocEvents_EquationEditorPostNotifyEventHandler(     System.bool Changed ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` public delegate System.int DDrawingDocEvents_EquationEditorPostNotifyEventHandler(  &   System.bool Changed ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Changed*
:   True if equations have changed, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See EquationEditorPostNotify Event (DrawingDoc).

# ![](dotnetimages/collapse.gif)Remarks

The IDrawingDoc event [EquationEditorPreNotify](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.DDrawingDocEvents_EquationEditorPreNotifyEventHandler.html) notifies your application that the equation editor has been constructed.

If developing a C++ application, use swDrawingEquationEditorPostNotify to register for this notification.

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2007 SP4, Revision Number 15.4