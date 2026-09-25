<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup~AddCommandItem.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| AddCommandItem Method (ICommandGroup) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [ICommandGroup Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup.html) : AddCommandItem Method (ICommandGroup) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*Name*

*Position*

*HintString*

*ToolTip*

*ImageListIndex*

*CallbackFunction*

*EnableMethod*

*UserID*

Obsolete. Superseded by [ICommandGroup::AddComandItem2](SOLIDWORKS.Interop.sldworks~SOLIDWORKS.Interop.sldworks.ICommandGroup~AddCommandItem2.html).

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function AddCommandItem( _    ByVal Name As System.String, _    ByVal Position As System.Integer, _    ByVal HintString As System.String, _    ByVal ToolTip As System.String, _    ByVal ImageListIndex As System.Integer, _    ByVal CallbackFunction As System.String, _    ByVal EnableMethod As System.String, _    ByVal UserID As System.Integer _ ) As System.Integer ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As ICommandGroup Dim Name As System.String Dim Position As System.Integer Dim HintString As System.String Dim ToolTip As System.String Dim ImageListIndex As System.Integer Dim CallbackFunction As System.String Dim EnableMethod As System.String Dim UserID As System.Integer Dim value As System.Integer   value = instance.AddCommandItem(Name, Position, HintString, ToolTip, ImageListIndex, CallbackFunction, EnableMethod, UserID) ``` | |

| C# |  |
| --- | --- |
| ``` System.int AddCommandItem(     System.string Name,    System.int Position,    System.string HintString,    System.string ToolTip,    System.int ImageListIndex,    System.string CallbackFunction,    System.string EnableMethod,    System.int UserID ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.int AddCommandItem(  &   System.String^ Name, &   System.int Position, &   System.String^ HintString, &   System.String^ ToolTip, &   System.int ImageListIndex, &   System.String^ CallbackFunction, &   System.String^ EnableMethod, &   System.int UserID ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*Name*

*Position*

*HintString*

*ToolTip*

*ImageListIndex*

*CallbackFunction*

*EnableMethod*

*UserID*

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See CommandGroup::AddCommandItem.

# ![](dotnetimages/collapse.gif)See Also

####

[ICommandGroup Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup.html)

[ICommandGroup Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.ICommandGroup_members.html)