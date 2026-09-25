<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITaskpaneView~DisplayWindowFromHandle.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| DisplayWindowFromHandle Method (ITaskpaneView) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ITaskpaneView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITaskpaneView.html) : DisplayWindowFromHandle Method (ITaskpaneView) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*WindowHandle*
:   Handle of .NET control

Adds a .NET control to the Task Pane view.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function DisplayWindowFromHandle( _    ByVal WindowHandle As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ITaskpaneView Dim WindowHandle As System.Integer Dim value As System.Boolean   value = instance.DisplayWindowFromHandle(WindowHandle) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool DisplayWindowFromHandle(     System.int WindowHandle ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool DisplayWindowFromHandle(  &   System.int WindowHandle ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*WindowHandle*
:   Handle of .NET control

#### Return Value

True if .NET control is added, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See TaskpaneView::DisplayWindowFromHandle.

# ![](dotnetimages/collapse.gif)Remarks

If your application must be x64 compatible, then use [ITaskPaneView::DisplayWindowFromHandlex64](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ITaskpaneView~DisplayWindowFromHandlex64.html).

# ![](dotnetimages/collapse.gif)See Also

####

[ITaskpaneView Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITaskpaneView.html)

[ITaskpaneView Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITaskpaneView_members.html)

[ITaskpaneView::AddControl Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ITaskpaneView~AddControl.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2011 FCS, Revision Number 19.0