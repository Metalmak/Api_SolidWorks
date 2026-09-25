<!-- source: toolboxapi/SolidWorks.Interop.sldtoolboxconfigureaddin~SolidWorks.Interop.sldtoolboxconfigureaddin.IToolboxConfiguratorAddin~Connect.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS Toolbox Browser API | Send Feedback |
| Connect Method (IToolboxConfiguratorAddin) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldtoolboxconfigureaddin Namespace](SolidWorks.Interop.sldtoolboxconfigureaddin~SolidWorks.Interop.sldtoolboxconfigureaddin_namespace.html) > [IToolboxConfiguratorAddin Interface](SolidWorks.Interop.sldtoolboxconfigureaddin~SolidWorks.Interop.sldtoolboxconfigureaddin.IToolboxConfiguratorAddin.html) : Connect Method (IToolboxConfiguratorAddin) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*pTbcApplication*
:   [IToolboxConfiguratorApplication](SOLIDWORKS.Interop.sldtoolboxconfigureaddin~SOLIDWORKS.Interop.sldtoolboxconfigureaddin.IToolBoxConfiguratorApplication.html)

*lCookie*
:   Add-in ID

Connects to the Welcome to Toolbox Setup dialog.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Function Connect( _    ByVal pTbcApplication As System.Object, _    ByVal lCookie As System.Integer _ ) As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IToolboxConfiguratorAddin Dim pTbcApplication As System.Object Dim lCookie As System.Integer Dim value As System.Boolean   value = instance.Connect(pTbcApplication, lCookie) ``` | |

| C# |  |
| --- | --- |
| ``` System.bool Connect(     System.object pTbcApplication,    System.int lCookie ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` System.bool Connect(  &   System.Object^ pTbcApplication, &   System.int lCookie ) ``` | |

#### Parameters

*pTbcApplication*
:   [IToolboxConfiguratorApplication](SOLIDWORKS.Interop.sldtoolboxconfigureaddin~SOLIDWORKS.Interop.sldtoolboxconfigureaddin.IToolBoxConfiguratorApplication.html)

*lCookie*
:   Add-in ID

#### Return Value

True if successful, false if not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ToolboxConfiguratorAddin::Connect.

# ![](dotnetimages/collapse.gif)See Also

####

[IToolboxConfiguratorAddin Interface](SolidWorks.Interop.sldtoolboxconfigureaddin~SolidWorks.Interop.sldtoolboxconfigureaddin.IToolboxConfiguratorAddin.html)

[IToolboxConfiguratorAddin Members](SolidWorks.Interop.sldtoolboxconfigureaddin~SolidWorks.Interop.sldtoolboxconfigureaddin.IToolboxConfiguratorAddin_members.html)

[IToolboxConfiguratorAddin::Disconnect Method](SolidWorks.Interop.sldtoolboxconfigureaddin~SolidWorks.Interop.sldtoolboxconfigureaddin.IToolboxConfiguratorAddin~Disconnect.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2013 FCS, Revision Number 21.0