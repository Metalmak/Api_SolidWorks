<!-- source: sldworksapi/SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo~IncludeToolboxComponents.html -->

![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/collapse.gif) ![](dotnetimages/expand.gif) ![](dotnetimages/drpdown.gif) ![](dotnetimages/drpdown_orange.gif) ![](dotnetimages/copycode.gif) ![](dotnetimages/copycodeHighlight.gif)

|  |  |
| --- | --- |
| SOLIDWORKS API Help | Send comments on this topic. |
| IncludeToolboxComponents Property (IPackAndGo) | |
| [See Also](#seealsobookmark)  [Example](#ExampleBookmark) | |

|  |
| --- |
| ![](dotnetimages/collapse.gif) Collapse All  Expand All ![](dotnetimages/drpdown.gif)  Language Filter: All Language Filter: Multiple Language Filter: Visual Basic (Declaration) Language Filter: Visual Basic (Usage) Language Filter: C# Language Filter: C++/CLI |

|  |
| --- |
| [SolidWorks.Interop.sldworks Namespace](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks_namespace.html) > [IPackAndGo Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo.html) : IncludeToolboxComponents Property (IPackAndGo) |

[ ]

Visual Basic (Declaration)

[ ]

Visual Basic (Usage)

[ ]

C#

[ ]

C++/CLI

Gets or sets whether to include SOLIDWORKS Toolbox components in Pack and Go.

# ![](dotnetimages/collapse.gif).NET Syntax

| Visual Basic (Declaration) |  |
| --- | --- |
| ``` Property IncludeToolboxComponents As System.Boolean ``` | |

| Visual Basic (Usage) | ![](dotnetimages/copycode.gif)Copy Code |
| --- | --- |
| ``` Dim instance As IPackAndGo Dim value As System.Boolean   instance.IncludeToolboxComponents = value   value = instance.IncludeToolboxComponents ``` | |

| C# |  |
| --- | --- |
| ``` System.bool IncludeToolboxComponents {get; set;} ``` | |

| C++/CLI |  |
| --- | --- |
| ``` property System.bool IncludeToolboxComponents {    System.bool get();    void set ( &   System.bool value); } ``` | |

**NOTE:** See [Differences Between Unmanaged C++ and C++/CLI Code](DifferencesBetweenUnManagedAndCPPCLI.htm).

#### Property Value

True to include SOLIDWORKS Toolbox components in Pack and Go, false to not

# ![](dotnetimages/collapse.gif)Visual Basic for Applications (VBA) Syntax

See PackAndGo::IncludeToolboxComponents.

# ![](dotnetimages/collapse.gif)Example

[Pack and Go an Assembly (C#)](Pack_and_Go_an_Assembly_Example_CSharp.htm)

[Pack and Go an Assembly (VB.NET)](Pack_and_Go_an_Assembly_Example_VBNET.htm)

[Pack and Go an Assembly (VBA)](Pack_and_Go_an_Assembly_Example_VB.htm)

# ![](dotnetimages/collapse.gif)See Also

####

[IPackAndGo Interface](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo.html)

[IPackAndGo Members](SolidWorks.Interop.sldworks~SolidWorks.Interop.sldworks.IPackAndGo_members.html)

# ![](dotnetimages/collapse.gif)Availability

SOLIDWORKS 2015 FCS, Revision Number 23.0