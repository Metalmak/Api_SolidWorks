<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~GetStatusBarPane.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| GetStatusBarPane Method (IFrame) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFrame Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame.html) : GetStatusBarPane Method (IFrame) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets a pointer to one of up to five panes on the right side of the status bar.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function GetStatusBarPane() As StatusBarPane ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFrame Dim value As StatusBarPane   value = instance.GetStatusBarPane() ``` | |

| C# |  |
| --- | --- |
| ``` StatusBarPane GetStatusBarPane() ``` | |

| C++/CLI |  |
| --- | --- |
| ``` StatusBarPane^ GetStatusBarPane(); ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Return Value

Pointer to a [status bar pane object](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IStatusBarPane.html)

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Frame::GetStatusBarPane.

# ![](dotnetimages/collapse.gif)Remarks

There are only 5 panes available starting from the right of the screen to the existing SOLIDWORKS panes.

This method returns a null pointer to a pane when you have used all possible panes.

These objects appear on the status bar until they go out of scope. To use them in a project, they should be declared globally in the Visual Basic project and managed during the life cycle of the client application.

# ![](dotnetimages/collapse.gif)See Also

####

[IFrame Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame.html)

[IFrame Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame_members.html)

[IFrame::SetStatusBarText Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~SetStatusBarText.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2001Plus FCS, Revision Number 10.0