<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame~AddMenuItem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddMenuItem Method (IFrame) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IFrame Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame.html) : AddMenuItem Method (IFrame) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Menu*

*Item*

*Position*

*CallbackFcnAndModule*

Obsolete. Superseded by [IFrame::AddMenuItem2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.IFrame~AddMenuItem2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddMenuItem( _    ByVal Menu As System.String, _    ByVal Item As System.String, _    ByVal Position As System.Integer, _    ByVal CallbackFcnAndModule As System.String _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IFrame Dim Menu As System.String Dim Item As System.String Dim Position As System.Integer Dim CallbackFcnAndModule As System.String Dim value As System.Boolean   value = instance.AddMenuItem(Menu, Item, Position, CallbackFcnAndModule) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool AddMenuItem(     System.string Menu,    System.string Item,    System.int Position,    System.string CallbackFcnAndModule ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool AddMenuItem(  &   System.String^ Menu, &   System.String^ Item, &   System.int Position, &   System.String^ CallbackFcnAndModule ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Menu*

*Item*

*Position*

*CallbackFcnAndModule*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See Frame::AddMenuItem.

# ![](dotnetimages/collapse.gif)See Also

####

[IFrame Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame.html)

[IFrame Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IFrame_members.html)