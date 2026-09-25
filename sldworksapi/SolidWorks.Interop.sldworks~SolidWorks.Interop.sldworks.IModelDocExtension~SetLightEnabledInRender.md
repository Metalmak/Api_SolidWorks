<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~SetLightEnabledInRender.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| SetLightEnabledInRender Method (IModelDocExtension) | |
| [See Also](#seealsobookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html) : SetLightEnabledInRender Method (IModelDocExtension) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

*ID*
:   Light ID

*Val*
:   True to enable the light, false to not

Sets whether a light is on in this model.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Sub SetLightEnabledInRender( _    ByVal ID As System.Integer, _    ByVal Val As System.Boolean _ ) ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IModelDocExtension Dim ID As System.Integer Dim Val As System.Boolean   instance.SetLightEnabledInRender(ID, Val) ``` | |

| C# |  |
| --- | --- |
| ``` void SetLightEnabledInRender(     System.int ID,    System.bool Val ) ``` | |

| C++/CLI |  |
| --- | --- |
| ``` void SetLightEnabledInRender(  &   System.int ID, &   System.bool Val ) ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Parameters

*ID*
:   Light ID

*Val*
:   True to enable the light, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See ModelDocExtension::SetLightEnabledInRender.

# ![](dotnetimages/collapse.gif)See Also

####

[IModelDocExtension Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension.html)

[IModelDocExtension Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension_members.html)

[IModelDocExtension::GetLightEnabledInRender Method](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IModelDocExtension~GetLightEnabledInRender.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2008 FCS, Revision Number 16.0