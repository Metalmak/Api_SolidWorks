<!-- source: toolboxapi/SolidWorks.Interop.sldtoolboxconfigureaddin~SolidWorks.Interop.sldtoolboxconfigureaddin.IToolBoxConfiguratorApplication~SendMessageToUser.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Toolbox Browser API | Send Feedback |
| SendMessageToUser Method (IToolBoxConfiguratorApplication) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldtoolboxconfigureaddin Namespace](SolidWorks.Interop.sldtoolboxconfigureaddin~SolidWorks.Interop.sldtoolboxconfigureaddin_namespace.html) > [IToolBoxConfiguratorApplication Interface](SolidWorks.Interop.sldtoolboxconfigureaddin~SolidWorks.Interop.sldtoolboxconfigureaddin.IToolBoxConfiguratorApplication.html) : SendMessageToUser Method (IToolBoxConfiguratorApplication) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*message*
:   Message string

Prompts the user with the specified message.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SendMessageToUser( _    ByVal message As System.String _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IToolBoxConfiguratorApplication Dim message As System.String   instance.SendMessageToUser(message) ``` | |

| C# |  |
| --- | --- |
| ``` void SendMessageToUser(     System.string message ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SendMessageToUser(  &   System.String^ message ) ``` | |

#### Parameters

*message*
:   Message string

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ToolBoxConfiguratorApplication::SendMessageToUser.

# ![](dotnetimages/collapse.gif)See Also

####

[IToolBoxConfiguratorApplication Interface](SolidWorks.Interop.sldtoolboxconfigureaddin~SolidWorks.Interop.sldtoolboxconfigureaddin.IToolBoxConfiguratorApplication.html)

[IToolBoxConfiguratorApplication Members](SolidWorks.Interop.sldtoolboxconfigureaddin~SolidWorks.Interop.sldtoolboxconfigureaddin.IToolBoxConfiguratorApplication_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0